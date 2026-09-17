# 培训日程卡网站

线上地址：http://121.5.21.95:8080/

此仓库的 `main` 分支是网站的发布来源。修改根目录的 `index.html` 并推送到 `main` 后，云服务器通常会在下一分钟自动拉取并发布新版本。无需手动登录服务器。

服务器上的网站运行在独立的 `zhibo-site` 服务和 8080 端口，不影响原有 80 端口服务。发布脚本位于 `/usr/local/sbin/deploy-zhibo-site`，定时配置位于 `/etc/cron.d/zhibo-site`，日志位于 `/var/log/zhibo-deploy.log`。
