# 本方法在微信最新版本2.6.8.51上使用会有一定概率造成微信撤回信息时闪退，请做好dll备份

# Wechat-Non-Revoke-Win10
PC端微信防撤回功能开发和实现

使用x32dbg对微信进行调试，找到revokemsg功能，将其删除，替换原有dll即可。

调试过程：
1. 打开x32dbg，管理员
2. 打开文件WeChat.exe
3. 下一步调试
4. 搜索进程 wechatwin.dll
5. 在模块内搜索revokemsg
6. 删去call
7. save

目前测试版本 2.6.7.40
