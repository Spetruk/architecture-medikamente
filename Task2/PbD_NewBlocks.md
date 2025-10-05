# Новые блоки целевой архитектуры (Privacy by Design)

- **Security & Privacy Layer (IDP MFA, Consent, PDP ABAC/RBAC)**: SSO/MFA, управление согласиями, решения по доступу на основе тегов/атрибутов.
- **Privacy/API Gateway**: единая точка входа; контракты, минимизация полей, фильтрация ответов, rate limiting, журналирование.
- **Core Services (EHR/CRM)**: управляемый доступ к медданным/клиентским данным; запись в защищённое хранилище объектов.
- **Payment Gateway**: разделение кассовых операций, минимизация реквизитов.
- **Integration Hub (Lab)**: безопасные контракты с лабораториями, mTLS, подпись.
- **Secure Storage (KMS/Vault)**: шифрование на покое, версии, аудит, управление доступом и ключами.
- **Privacy‑aware Data Platform (включая Data Catalog & Lineage и Privacy Services)**: витрины, изоляция PII/HEALTH, политики доступа; каталог/lineage; псевдонимизация/обезличивание/маскирование для аналитики/выдач.
- **Security Monitoring (SIEM)**: сбор аудита, корреляция, алерты.

# Аналитический слой (Privacy-aware)
- Источник: CDC/ETL из EHR/CRM/1С/почты/лаборатории.
- Защита: обезличивание/маскирование (Privacy Services), ключи в KMS/Vault.
- Управление: Data Catalog & Lineage с тегами и сроками хранения.
- Доступ: ABAC через PDP (в составе Security & Privacy Layer), аудит доступа в SIEM.

# Соответствие диаграмме
- Security & Privacy Layer — блок «Security & Privacy Layer».
- Privacy/API Gateway — блок «Privacy/API Gateway».
- Core Services — блок «Core Services (EHR/CRM)».
- Payment Gateway — блок «Payment Gateway».
- Integration Hub — блок «Integration Hub (Lab)».
- Secure Storage (KMS/Vault) — блок «Secure Storage (KMS)».
- Data Platform — блок «Privacy-aware Data Platform».
- SIEM — блок «Security Monitoring (SIEM)».
