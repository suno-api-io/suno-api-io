# Suno-API Developer

Independent third-party AI music platform and developer API for Suno V6-series
generation.

> Suno-API is not affiliated with Suno. The GitHub account publishes developer
> examples, integration notes, and reproducible troubleshooting material for the
> independent Suno-API service.

## Build with the API

- **Website:** https://www.suno-api.io/
- **Create music in the browser:** https://www.suno-api.io/create/
- **API documentation:** https://www.suno-api.io/docs/
- **Python starter:** https://github.com/a649045484-ux/suno-api-python-starter

## What the starter demonstrates

- asynchronous generation acceptance;
- idempotency keys for safe retries;
- bounded polling instead of infinite retry loops;
- explicit distinction between `request_id`, task index, and `song_id`;
- safe handling of short-lived media URLs;
- a small CI workflow with no real credentials.

## Integration principles

1. Keep API keys on the server.
2. Retry only errors that are safe to retry.
3. Treat accepted, processing, completed, and failed as different states.
4. Persist request IDs and task IDs separately.
5. Download and re-host media before short-lived URLs expire.
6. Never post keys, cookies, private media, or user data in an issue.

## 中文入口

Suno-API 是独立第三方 AI 音乐平台和开发者 API，接入 Suno V6 系列音乐生成能力，与 Suno 官方无隶属关系。

- 官网：https://www.suno-api.io/
- 在线创作：https://www.suno-api.io/create/
- 开发者文档：https://www.suno-api.io/docs/
- Python 示例：https://github.com/a649045484-ux/suno-api-python-starter

