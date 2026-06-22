# CFnew Deployer

本地部署软件，支持 Cloudflare Worker 和 Pages。

## 启动

```bash
npm start
```

打开 `http://localhost:8790`。

## 支持能力

- 用户填写 Cloudflare 邮箱和 Global API Key
- 自动读取账户和可绑定域名
- 默认随机生成项目名称和 KV 名称
- 自动生成 UUID
- 自动创建或复用 KV，并绑定为 `C`
- 支持读取现有 Worker / Pages / KV 后更新部署
- 更新部署只同步代码，不修改 UUID、KV、域名或项目配置
- Worker 部署
- Pages 部署
- 明文源 `sources/明文源吗` 或混淆源 `sources/少年你相信光吗`
- Worker 自定义域名或 Route 绑定
- Pages 自定义域名绑定

密钥只在本地 Node 进程内使用，不会写入文件或浏览器 localStorage。
