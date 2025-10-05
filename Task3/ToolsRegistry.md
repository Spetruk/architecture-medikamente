# Реестр программных и аппаратных средств защиты данных

## Шифрование и управление ключами
- KMS (облако/on‑prem), HashiCorp Vault — генерация/хранение/ротация ключей, KMIP/HSM.
- HSM (аппаратный модуль безопасности) — хранение корневых ключей, операции подписи.

## Контроль доступа и политики
- Identity Provider (OIDC/OAuth2, MFA) — SSO.
- PDP/OPA — решения ABAC/RBAC по тегам/контексту.

## Мониторинг и аудит
- SIEM — сбор логов доступа/изменений, корреляция и алерты.
- File Integrity Monitoring — контроль целостности файлов/конфигураций.

## DLP и почтовая безопасность
- Exchange/O365 DLP, Transport Rules, S/MIME — контроль и шифрование вложений.

## API и интеграции
- API Gateway — rate limiting, schema validation, authz, mTLS.
- Integration Hub — безопасные коннекторы к лаборатории и 1С.

## Хранилища и резервное копирование
- Secure Object Storage — Encrypt‑at‑Rest, версии, WORM.
- Backup/DR — шифрование бэкапов, изоляция, тесты восстановления.

## Каталог и lineage
- Data Catalog & Lineage — OpenMetadata/Amundsen/DataHub.

## Маскирование/обезличивание
- Privacy Services — статическое/динамическое маскирование, токенизация, псевдонимизация.
