# Suno-API Developer

[简体中文](#简体中文) | [English](#english) | [日本語](#日本語) | [Français](#français) | [Русский](#русский)

📚 [完整 GitHub 接口文档 / Complete API documentation](https://github.com/suno-api-io/suno-api-python-starter/blob/main/docs/README.md)

🧭 [媒体交付指南 / Media delivery guide](https://github.com/suno-api-io/suno-api-python-starter/blob/main/guides/media-url-lifecycle.md)

## Technical writing

- [AI 音乐 API 接入失败地图（CSDN）](https://blog.csdn.net/qq_15889541111/article/details/170122909)
- [AI 音乐生成完成后的媒体交付（CSDN）](https://blog.csdn.net/qq_15889541111/article/details/170346504)
- [AI 音乐 API 超时与故障排查（知乎）](https://zhuanlan.zhihu.com/p/2101601083139286737)

## 简体中文

AI 音乐平台和开发者 API，使用 Suno 官方 V6 模型。

这个 GitHub 账号发布开发者示例、接入说明和可复现的故障排查资料。

### 开始使用

- 官网：https://www.suno-api.io/
- 在线创作：https://www.suno-api.io/create/
- API 文档：https://www.suno-api.io/docs/
- Python 示例：https://github.com/suno-api-io/suno-api-python-starter

### Python 示例包含

- 异步生成受理；
- 安全重试与幂等键；
- 有界轮询；
- `request_id`、任务序号和 `song_id` 的分层管理；
- 短期媒体 URL 与文件交付；
- 不包含真实凭证的 CI 流程。

### 接入原则

1. API Key 只保存在服务端。
2. 只重试适合重试的错误。
3. 分别记录受理、处理中、完成和失败状态。
4. 分别保存受理号和歌曲 ID。
5. 在短期媒体 URL 到期前完成转存。
6. 不在公开 Issue 中发送 Key、Cookie、私有媒体或用户数据。

## English

An AI music platform and developer API powered by official Suno V6 models.

This GitHub account publishes developer examples, integration notes, and reproducible troubleshooting material.

### Get started

- Website: https://www.suno-api.io/
- Create music: https://www.suno-api.io/create/
- API documentation: https://www.suno-api.io/docs/
- Python starter: https://github.com/suno-api-io/suno-api-python-starter

### What the Python starter demonstrates

- asynchronous generation acceptance;
- safe retries with idempotency keys;
- bounded polling;
- separate management of `request_id`, task index, and `song_id`;
- short-lived media URLs and delivery checks;
- a CI workflow with no real credentials.

### Integration principles

1. Keep API keys on the server.
2. Retry only errors that are safe to retry.
3. Treat accepted, processing, completed, and failed as different states.
4. Persist request IDs and song IDs separately.
5. Re-host media before short-lived URLs expire.
6. Never post keys, cookies, private media, or user data in a public issue.

## 日本語

Suno 公式 V6 モデルを使用する AI 音楽プラットフォームおよび開発者向け API です。

この GitHub アカウントでは、開発者向けサンプル、連携ガイド、再現可能なトラブルシューティング資料を公開しています。

### はじめに

- ウェブサイト：https://www.suno-api.io/
- 楽曲作成：https://www.suno-api.io/create/
- API ドキュメント：https://www.suno-api.io/docs/
- Python サンプル：https://github.com/suno-api-io/suno-api-python-starter

### Python サンプルの内容

- 非同期の生成受付；
- 冪等キーを使用した安全な再試行；
- 上限付きポーリング；
- `request_id`、タスク番号、`song_id` の分離管理；
- 短期間有効なメディア URL とファイル配信；
- 実際の認証情報を含まない CI ワークフロー。

### 連携の原則

1. API キーはサーバー側だけで保管します。
2. 再試行しても安全なエラーのみを再試行します。
3. 受付済み、処理中、完了、失敗を別の状態として扱います。
4. 受付 ID と楽曲 ID を別々に保存します。
5. 短期メディア URL の有効期限前にファイルを保存します。
6. 公開 Issue にキー、Cookie、非公開メディア、ユーザーデータを投稿しないでください。

## Français

Une plateforme de musique par IA et une API pour développeurs basées sur les modèles officiels Suno V6.

Ce compte GitHub publie des exemples pour développeurs, des notes d'intégration et des documents de résolution de problèmes reproductibles.

### Pour commencer

- Site web : https://www.suno-api.io/
- Création musicale : https://www.suno-api.io/create/
- Documentation API : https://www.suno-api.io/docs/
- Exemple Python : https://github.com/suno-api-io/suno-api-python-starter

### Contenu de l'exemple Python

- acceptation asynchrone de la génération ;
- nouvelles tentatives sûres avec des clés d'idempotence ;
- interrogation limitée ;
- gestion séparée de `request_id`, de l'index de tâche et de `song_id` ;
- URL de média temporaires et livraison des fichiers ;
- workflow CI sans identifiants réels.

### Principes d'intégration

1. Conservez les clés API uniquement côté serveur.
2. Ne relancez que les erreurs qui peuvent l'être sans risque.
3. Distinguez les états accepté, en cours, terminé et échoué.
4. Enregistrez séparément les identifiants de requête et de morceau.
5. Copiez les médias avant l'expiration des URL temporaires.
6. Ne publiez jamais de clés, cookies, médias privés ou données utilisateur dans une issue publique.

## Русский

Платформа музыки с помощью ИИ и API для разработчиков на основе официальных моделей Suno V6.

Этот аккаунт GitHub публикует примеры для разработчиков, руководства по интеграции и воспроизводимые материалы по устранению неполадок.

### Начало работы

- Сайт: https://www.suno-api.io/
- Создание музыки: https://www.suno-api.io/create/
- Документация API: https://www.suno-api.io/docs/
- Пример на Python: https://github.com/suno-api-io/suno-api-python-starter

### Что содержит пример на Python

- асинхронный приём запросов на генерацию;
- безопасные повторные запросы с ключами идемпотентности;
- ограниченный опрос статуса;
- раздельное управление `request_id`, индексом задачи и `song_id`;
- краткосрочные URL медиафайлов и проверка доставки;
- рабочий процесс CI без реальных учётных данных.

### Принципы интеграции

1. Храните ключи API только на сервере.
2. Повторяйте только те ошибки, для которых повторный запрос безопасен.
3. Различайте состояния принято, обрабатывается, завершено и ошибка.
4. Сохраняйте идентификаторы запроса и композиции отдельно.
5. Копируйте медиафайлы до истечения срока действия краткосрочных URL.
6. Никогда не публикуйте ключи, cookie, закрытые медиафайлы или пользовательские данные в открытых issue.
