```
左手备忘录
```
* ~~sqlite存储memo~~	
* ~~蓝牙推送到glass~~
* ~~上传memo到服务器~~
* ~~添加删除memo功能~~

---

```
Glass备忘录
```
* ~~后台service(开机启动)，监听广播(包含memo对象)~~
* ~~`service 启动时` 或者 `接收到memo时`，`检查数据库中的备忘录`，把`当天的备忘录`加入到AlarmManager~~
* ~~收到memo后：`存到sqlite中` 、`创建定时任务`~~
* ~~主界面：用viewPager做，初始化时查询出当天的todo，排序，
左边(...过时任务)|当前(第一个未来任务)|右边(第二个未来任务...)~~
* ~~添加memo删除功能~~

---


```
蓝牙接收端 done
```
* ~~接收Proto.Memo~~
* ~~发送广播通知Glass备忘录（memo）~~

protoc --java_out=./memo/src/main/java/ --proto_path=./memo/src/main/proto/ ./memo/src/main/proto/*.proto

---
