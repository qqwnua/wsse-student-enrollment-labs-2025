# Lab 02 Submission

## 1. Repo 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025](https://github.com/qqwnua/wsse-student-enrollment-labs-2025)

## 2. PR 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/2](https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/2)

## 3. Cognito 設定截圖
### User Pool 資訊
![User Pool Info](../images/lab02/01-cognito-pool.png)

### App Client Domain
![Cognito Domain](../images/lab02/02-cognito-domain.png)

### App Client 詳細設定 (No Secret & Callback)
![App Client Config](../images/lab02/03-cognito-appclient.png)

### Resource Server Scopes
![Scopes](../images/lab02/04-cognito-scopes.png)

## 4. Token 驗證截圖 (JWT)
### Access Token 解析 (含 Scope)
![JWT Claims](../images/lab02/05-jwt-access-claims.png)

## 5. CI/CD 截圖
### Swagger Editor 無錯誤驗證
![OpenAPI Valid](../images/lab02/06-editor-no-errors.png)

### PR 綠燈截圖
![PR Green](../images/lab02/07-pr-ci-green.png)

## 6. OpenAPI 重點片段連結
* [openapi/openapi.yaml](/openapi/openapi.yaml) - OAuth2 Security Scheme Definition (components)
* [openapi/openapi.yaml](/openapi/openapi.yaml) - Global Security Requirement (security)
