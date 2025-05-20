# FireDetection Kafka Consumer

🔥 Kafka 기반 화재 감지 시스템의 데이터 수신 및 처리 컴포넌트입니다.

## 📌 개요

이 Kafka Consumer는 화재 감지 센서로부터 전송되는 실시간 데이터를 수신하고, 이를 분석하여 화재 발생 여부를 판단하거나 후속 시스템에 전달하는 역할을 합니다.

---

## 📦 주요 기능

- Kafka 토픽(`fire-detection-event`)
- JSON 기반 센서 데이터 파싱
- 데이터 정합성 검증
- 알림 시스템 연계 (Webhook / DB 저장 등)

---

## ⚙️ 시스템 구조

```
Kafka Producer (센서)
        ↓
[Kafka Topic: fire-detection-event]
        ↓
FireDetection Kafka Consumer
        ↓
[분석 및 저장 / 알림 연동]
```
