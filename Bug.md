# 已知 Bug 列表

最后编辑于 2018年5月11日下午

* 在部分系统上会时不时弹 QQ 停止运行的对话框、闪退，暂时没有找到原因
* 不开启有关 QQ 空间的任何功能空间也会有空间闪退的可能，暂时没有找到原因
* 在 VirtualXposed 里面点击看点和微视后 QQ 无响应是 VirtualXposed 的原因
* 隐藏消息列表顶部搜索框会下拉刷新的提示会往上有点偏移，凑合着用吧
* 隐藏侧栏厘米秀同时也会隐藏城市和天气
* 设置空白间隔，这个暂时不要吐槽谢谢合作

> 以上内容基本是以按影响程度排序

## 解决方法

> 此方法不保证一定能解决你的问题，我自认为感觉比以前稳定了点所以分享出来让大家试试

1. 完全退出 QQ

2. 在模块里面开启**高级功能-拦截热修复**

3. 打开 */data/data/com.tencent.mobileqq/*  删除此目录下的 *app_installed_plugin* 和 *app_odex* 文件夹

> VirtualXposed 用户找这个目录：*/data/data/io.va.exposed/virtual/data/user/0/com.tencent.mobileqq/*

PS：删除该目录后 QQ 会重新下载一遍补丁文件，所以会消耗一些流量，第一次进空间有点慢就是因为在下载文件