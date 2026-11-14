# Максим — junior бизнес-аналитик (процессы и требования + системный анализ)

Учусь и собираю **учебные кейсы** в финтехе и корпоративных финансах. Все проекты учебные: компании вымышленные, данные синтетические или открытые, внедрения не было. Ищу стажировку или junior-позицию BA/SA.

## Избранные кейсы

| Кейс | Проблема в одной фразе | Что показывает |
|---|---|---|
| [Согласование счетов с 1С и сверка с выпиской](https://github.com/MonsterOfBI/invoice-approval-1c) | Вымышленная торговая компания согласует счета в Excel и мессенджерах, платит пени и дубли. | BPMN, DMN, интервью, user stories, ER/SQL, интеграция с 1С, ROI |
| [Оплата в интернет-магазине: карта, QR СБП, цифровой рубль, возвраты](https://github.com/MonsterOfBI/online-payments) | Системный кейс на тестовом магазине ЮKassa: платёж, webhook, чек 54-ФЗ, возврат. | REST/OpenAPI, идемпотентность, webhooks, sequence/state, Postman, платёжный домен |
| [Проверка контрагента и кредитный лимит на данных ФНС](https://github.com/MonsterOfBI/counterparty-check) | Автопроверка новых контрагентов на реальных открытых данных ФНС: загрузка XML в PostgreSQL, скоринг правилами, лимит отсрочки, API и дашборд. | SQL CTE/окна, pandas, DMN, OpenAPI, DataLens, открытые данные |
| [Финансовый ассистент для ИП](https://github.com/MonsterOfBI/sme-finance-assistant) | Требования к LLM-фиче для ИП (автокатегоризация операций, платёжный календарь, подсказки) и замер её качества на 200 размеченных операциях. | требования к LLM, метрики качества, BRD, pandas, OpenAPI |

## Мини-кейсы (каждый — свой навык)

Все мини-кейсы лежат в одном репозитории [ba-mini-cases](https://github.com/MonsterOfBI/ba-mini-cases), каждый в своей папке.

### Платежи и банк
| Кейс | Навык |
|---|---|
| [Ключевая ставка ЦБ и пересчёт плавающих кредитов](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m3-key-rate-loans) | SOAP/WSDL, бизнес-правила, SQL |
| [Разбор антифрод-алертов](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m5-antifraud-alerts) | DataLens, SQL, метрики процесса |
| [Кэшбэк по категориям MCC](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m6-mcc-cashback) | DMN, генерация тестовых данных, SQL |
| [KYC-онбординг ИП по 115-ФЗ](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m8-kyc-onboarding) | регуляторные требования, DMN, KPI |

### Корпоративные финансы
| Кейс | Навык |
|---|---|
| [Авансовые отчёты сотрудников](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m1-expense-reports) | BPMN, user stories, DMN |
| [Курсы ЦБ и валютная переоценка](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m2-fx-revaluation) | XML/XSD, pandas, SQL |
| [Дебиторка: напоминания, aging и DSO](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m4-receivables-dso) | SQL CTE/окна, BPMN таймеры |
| [БДДС и платёжный календарь в Excel](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/m7-cash-flow-budget) | Excel, БДДС, финансовый словарь |

### Вне финансов
| Кейс | Навык |
|---|---|
| [Возврат товара на маркетплейсе](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/n1-marketplace-returns) | BPMN, SQL на чужой схеме |
| Заявка на отпуск (кейс на время) *(в работе: появится после первой попытки)* | выявление требований, BPMN, тайм-боксинг |
| [Интеграция CRM ↔ 1С: от лида до счёта](https://github.com/MonsterOfBI/ba-mini-cases/tree/main/n3-crm-1c-integration) | интеграции, маппинг данных, sequence |

## Навыки (честно)

| Навык | Уровень | Где посмотреть |
|---|---|---|
| BPMN 2.0, DMN (Camunda Modeler) | применяю | Ф1, М1, Н1 |
| User stories, Given/When/Then, НФТ | применяю | Ф1, Ф2, М1 |
| SQL (PostgreSQL): JOIN, CTE, оконные функции | учусь, применяю в кейсах | Ф1, Ф2, М4 |
| REST, OpenAPI, идемпотентность, Postman | учусь | Ф2, Н3 |
| Интеграции, очереди (понятийно), sequence | учусь | Ф1, Ф2, Н3 |
| Финансы: бухучёт (базово), платежи, СБП | учусь | Ф1, Ф2, М2 |

## Как я работаю с ИИ
ИИ-ассистент (Claude) — тренажёр и ревьюер: играет стейкхолдеров на учебных интервью, генерирует синтетические данные, делает ревью. Первые версии кейсов собраны вместе с ним; что я переделал и проверил сам — в разделе «Как сделано» и в `DEFENSE.md` каждого репозитория. Кейс «Заявка на отпуск» решаю без ИИ, на время.
