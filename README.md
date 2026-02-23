# peizhi
三国杀ol和一将成名的解密后配置文件  通过cloudflare的kv缓存实现有更新就下载 这个配置包含了所有必需的内容：

✅ Worker 名称和入口文件
✅ 兼容性日期
✅ 定时任务（每 5 分钟检查更新）
✅ KV 命名空间配置
这样 Worker 会：

每 5 分钟自动检查三国杀配置文件是否更新
如果有更新，下载并缓存到 KV
提供解密后的文件给 GitHub Actions 下载
给了cloudflare   git仓库的key一个月有效期
