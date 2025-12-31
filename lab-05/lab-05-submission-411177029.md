# Lab 05 Submission

## 1. Repo 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025](https://github.com/qqwnua/wsse-student-enrollment-labs-2025)

## 2. PR 連結
[https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/5](https://github.com/qqwnua/wsse-student-enrollment-labs-2025/pull/5)

## 3. 架構設定 (Infrastructure)
### SNS Topic 設定 (發布者)
![SNS Topic](./evidence/411177029-sns-topic.png)

### SQS Queue 設定 (訂閱者)
![SQS Queue](./evidence/411177029-sns-queue.png)

## 4. Lambda 設定 (Configuration)
### Producer Lambda (API) 環境變數
**說明：** 設定 `SNS_TOPIC_ARN` 以便發送訊息。
![Producer Config](./evidence/411177029-lambda-producer.png)

### Consumer Lambda (Event Processor) 觸發器
**說明：** 設定 SQS Trigger 以接收並處理訊息。
![Consumer Trigger](./evidence/411177029-lambda-consumer.png)

## 5. 測試結果驗證 (Testing)

### 1) API POST 測試 (觸發事件)
**預期結果：** HTTP 201 Created，且回應訊息包含 "event published"。
![API POST Result](./evidence/411177029-api-post-201.png)

### 2) CloudWatch Logs (接收事件)
**預期結果：** Consumer Lambda 成功印出從 SQS 收到的學生資料。
![CloudWatch Logs](./evidence/411177029-logs.png)