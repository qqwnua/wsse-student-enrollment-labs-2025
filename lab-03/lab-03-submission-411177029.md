# Lab 03 Submission

## 1. Repo 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025](https://github.com/qqwnua/wsse-student-enrollment-labs-2025)

## 2. PR 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/3](https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/3)

## 3. API Gateway 基礎設定 (Resources & Stage)
### Resources 樹狀圖 (顯示 /health 與 /students)
![Resources Tree](./evidence/411177029-api-resources.png)

### Stage prod 資訊 (顯示 Invoke URL)
![Stage Prod](./evidence/411177029-api-stage-prod.png)

### CORS 設定 (OPTIONS 方法或設定畫面)
![CORS Settings](./evidence/411177029-api-cors-students.png)

## 4. Lambda 整合設定 (Integration)
### Integration Request: GET /students (連結到 Lambda)
![Integration GET](./evidence/411177029-api-integration-get-students.png)

### Integration Request: POST /students (連結到 Lambda)
![Integration POST](./evidence/411177029-api-integration-post-students.png)

### Integration Request: GET /health (連結到 Lambda)
![Integration Health](./evidence/411177029-api-integration-health.png)

## 5. 安全性與授權設定 (Security & Scopes)
### Authorizer 設定 (Cognito Authorizer)
![Authorizer Config](./evidence/411177029-auth-authorizer.png)

### Scope 設定: GET Method Request (read scope)
![Scope GET](./evidence/411177029-auth-scope-get.png)

### Scope 設定: POST Method Request (write scope)
![Scope POST](./evidence/411177029-auth-scope-post.png)

## 6. 測試結果截圖 (Testing Evidence)
### Lambda 內部測試 A: /health (Execution result: succeeded)
![Lambda Test Health](./evidence/411177029-lamda-test-health.png)

### Lambda 內部測試 B: POST /students (Execution result: succeeded)
![Lambda Test POST](./evidence/411177029-lamda-test-post.png)

### CloudWatch Logs (證明 Curl 請求已進入)
![CloudWatch Logs](./evidence/411177029-logs.png)