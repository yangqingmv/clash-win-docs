## 常见问题

**1. 界面显示不全，无法操作**

删除 Home Directory 下 config.yaml 文件并重启软件
如错误依旧，打开 logs 文件夹，选取最新日志文件分析

**2. 升级后提示 xxx not found**

0.6.0 版本升级后，Clash 核心增加对规则部分的校验，如果策略不存在，则不再忽略而提示错误，根据错误信息检查配置文件并进行排除即可

**3. 系统代理自动关闭或打开**

清除系统代理设置
如无法解决，则检查是否有其他安全/代理软件修改代理设置

**4. 无法访问网页**

0.6.0 版本升级后，Clash 核心使用自定义 DNS 设置进行服务器及直连域名的解析，所以当日志中出现大量 All DNS Failed! 日志时，请重新设置合适的 DNS

如果不使用 TAP ，建议将 DNS 关闭

**5. TAP 无法安装**

检查是否已经安装其他 TAP 设备，若是，可以先在设备管理器中将其删除后重试