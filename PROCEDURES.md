# Полный каталог процедур TechStream — со ссылками на статьи

Для каждой процедуры указан:
- **Меню** в TechStream;
- **Назначение**;
- **Прямая ссылка на внешнюю пошаговую статью** со скриншотами или фото (форум, PDF-бюллетень Toyota, блог).

> ⚠️ Названия пунктов меню и доступность функций зависят от модели, года выпуска и версии TechStream. Авторитетный источник — Toyota TIS (techinfo.toyota.com) и ремонтный мануал конкретной модели.

---

## 0. База — установка, подключение, работа с ПО

| # | Процедура | Меню | Пошаговая статья со скриншотами |
|---|-----------|------|-------------------------------|
| 0.1 | Установка TechStream на Windows 10/11 x64 | — | [Drive2 — Установка на Windows 7/8.1/10 x64](https://www.drive2.ru/b/479152325051547873/) · [newhilux.net — Intro & HOW-TO](https://www.newhilux.net/phpbb/viewtopic.php?p=289699) |
| 0.2 | Решение ошибки «MVCI Driver ended prematurely» | — | [RTS Auto PDF](https://www.rtsauto.com/wp-content/uploads/2019/10/MVCI-Driver-ended-prematurely-error.pdf) |
| 0.3 | Решение «unable to connect to VIM» | — | [SlideShare — fix MVCI unable to connect](https://www.slideshare.net/slideshow/how-to-fix-mvci-techstream-unable-to-connect-to-vim/38691426) · [PriusChat — inconsistencies](https://priuschat.com/goto/post?id=2444747) |
| 0.4 | Первое подключение, выбор модели | *Main → Connect to Vehicle* | [Toyota Owners Club — connect laptop to OBD](https://toyotaownersclub.com/forums/topic/156801-how-to-connect-your-laptop-to-the-obd-socket) · [PriusChat — proper procedure](https://priuschat.com/goto/post?id=2160919) |
| 0.5 | Health Check (быстрое сканирование всех ECU) | *Function → Health Check* | [Toyota TSB SB-10060691-2280 (PDF)](https://static.nhtsa.gov/odi/tsbs/2014/SB-10060691-2280.pdf) |

---

## 1. Powertrain — двигатель и АКПП

### 1.1. Engine and ECT

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 1.1 | Чтение / сброс DTC | *Trouble Codes → Clear DTC* | [Toyota TSB SB-10062028-2280 (PDF)](https://static.nhtsa.gov/odi/tsbs/2013/SB-10062028-2280.pdf) · [TSB MC-10132450-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2017/MC-10132450-9999.pdf) |
| 1.2 | Reset Memory — сброс адаптации АКПП | *Engine and ECT → Utility → Reset Memory* | [Drive2 — сброс адаптации](https://www.drive2.ru/l/593361071729814017/) · [Drive2 — опыт на TLC Prado](https://www.drive2.ru/l/707437327256921961/) |
| 1.3 | AT Initialization | *Utility → AT Initialization* | [ClubLexus — Techstream](https://www.clublexus.com/forums/ls-4th-gen-2007-2017/910649-techstream.html) · [Drive2 — различия Reset/Init](https://www.drive2.ru/l/566077790198169720/) |
| 1.4 | Инициализация дроссельной заслонки | *Utility → Throttle Position Reset* | [Toyota Owners Club — throttle re-learn](https://toyotaownersclub.com/forums/topic/195291-throttle-re-learn-procedure) · [TPautoRepair — ETC reset](https://tpautorepair.net/how-do-i-reset-the-electronic-throttle-control/) |
| 1.5 | Регистрация ECM ID (после замены ЭБУ) | *Utility → ECM Communication ID Registration* | [Toyota TSB SB-10060732-2280 (PDF)](https://static.nhtsa.gov/odi/tsbs/2014/SB-10060732-2280.pdf) |
| 1.6 | Прописка форсунок (Injector Compensation) | *Utility → Injector Compensation* | [Toyota Owners Club — D-4D injector problems](https://toyotaownersclub.com/forums/topic/65603-05-20-d4d-injector-problems) · [AU7O — P1238 Toyota](https://au7o.io/known-issues/dtc/p1238/toyota) |
| 1.7 | VVT Learning Value Clear | *Utility → VVT Learn Clear* | [Toyota Owners Club — Techstream related](https://toyotaownersclub.com/forums/topic/187925-techstream-related-question) |
| 1.8 | Fuel Pump Learn Value | *Utility → Fuel Pump Learn* | [Toyota TSB — Control Injection Mode (PDF)](https://static.nhtsa.gov/odi/tsbs/2022/MC-10213896-9999.pdf) |
| 1.9 | Active Test — Control Injection Mode (FKS-двигатели) | *Active Test → Injection Mode* | [Toyota TSB MC-10213896-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2022/MC-10213896-9999.pdf) |
| 1.10 | Active Test — Fuel Pump / Cooling Fan / Injector | *Active Test → …* | [YouCanic — active test glossary](https://www.youcanic.com/glossary/active-test/) |
| 1.11 | EVAP Leak Test | *Utility → EVAP Leak Check* | [Toyota TSB MC-10201394-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2021/MC-10201394-9999.pdf) |
| 1.12 | Battery Reset / Current Sensor Initialization | *Utility → Battery Reset* | [PriusChat — reset ABS & yellow (!)](https://www.priuschat.com/goto/post?id=2825983) |

### 1.2. Cruise Control / Pre-Collision / ACC

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 1.13 | Калибровка переднего радара (Millimeter Wave) | *Powertrain → Pre-Collision 2 → Utility → Beam Axis Adjust* | [Automotive Tech Info — Toyota ADAS radar](https://automotivetechinfo.com/2021/08/radar-in-the-trenches-how-to-get-started-with-toyota-advanced-driver-assistance-systems-adas) · [Repairer Driven News — radar calibration](https://www.repairerdrivennews.com/2018/09/10/toyota-collision-pros-radar-must-be-calibrated-after-some-common-rrs-ris/) |
| 1.14 | Калибровка передней камеры (TSS) | *Body → Front Camera → Utility → Camera Learn* | [Fenderbender — Toyota/Lexus radar & camera calibration](https://fenderbender.com/news/article/55043242/free-webinar-from-ase-toyota-and-lexus-millimeter-wave-radar-and-front-recognition-camera-calibration) |

---

## 2. Chassis — ходовая, ABS, рулевое

### 2.1. ABS / VSC / TRAC

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 2.1 | Reset Memory | *Chassis → ABS/VSC/TRAC → Utility → Reset Memory* | [ClubLexus — zero point via Techstream](https://www.clublexus.com/forums/ls-3rd-gen-2001-2006/789241-how-to-do-a-zero-point-calibration-via-techstream.html) |
| 2.2 | Test Mode (вход в сервисный режим) | *Utility → Test Mode* | [vehicleservicepros — Toyota zero point TSB](https://www.vehicleservicepros.com/tsbs/article/53092346/toyota-zero-point-calibration-2014-10-06) |
| 2.3 | Zero Point Calibration (Yaw/G) | *Utility → Zero Point Calibration* | [PriusChat PDF — Prius SM Yaw/G](https://attachments.priuschat.com/attachment-files/2024/05/250911_Prius_SM_-_Yaw_Rate_and_Acceleration_Zero_Point.pdf) · [PriusChat PDF — Tundra manual reset](https://attachments.priuschat.com/attachment-files/2018/05/146139_Tundra_-_zero_point_manual_reset.pdf) |
| 2.4 | Прокачка тормозов — Air Bleeding | *Active Test → Air Bleeding* | [PriusChat — bleeding brakes with Techstream](https://www.priuschat.com/goto/post?id=2862028) · [ih8mud — ABS solenoid bleed](https://forum.ih8mud.com/threads/techstream-abs-solenoid-bleed.1279195) |
| 2.5 | ABS Motor Active Test | *Active Test → ABS Motor* | [Toyota TSB MC-10220187-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2022/MC-10220187-9999.pdf) |
| 2.6 | ECB — Linear Solenoid Valve Calibration | *Utility → Linear Valve Offset Learn* | [PriusChat PDF — Electronically Controlled Brake](https://attachments.priuschat.com/attachment-files/2022/05/221890_Electronically_controlled_brake_system.pdf) |
| 2.7 | ECB — Stroke Sensor / MC Pressure Zero Point | *Utility → Stroke Sensor Zero Point* | [PriusChat PDF — ECB system](https://attachments.priuschat.com/attachment-files/2022/05/221890_Electronically_controlled_brake_system.pdf) |

### 2.2. EPS — электроусилитель руля

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 2.8 | Torque Sensor Zero Point | *Chassis → EPS → Utility → Torque Sensor Zero* | [Toyota TSB MC-10177772-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2020/MC-10177772-9999.pdf) · [TechTips.ie — Corolla ESP torque reset (PDF)](https://www.techtips.ie/Ryans_Automotive/resetting-a-corolla-esp-torque-sensor.pdf) |
| 2.9 | Rotation Angle Sensor Calibration | *Utility → Rotation Angle Learn* | [TechTips.ie — та же PDF](https://www.techtips.ie/Ryans_Automotive/resetting-a-corolla-esp-torque-sensor.pdf) |
| 2.10 | Assist Map Writing (после замены ЭБУ) | *Utility → Assist Map* | [Toyota TSB MC-10220230-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2022/MC-10220230-9999.pdf) |

### 2.3. VGRS — переменное передаточное отношение

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 2.11 | Инициализация VGRS (руль по центру + поездка) | — | [Toyota TSB MC-10109460-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2014/MC-10109460-9999.pdf) · [ih8mud — off-center steering VGRS](https://forum.ih8mud.com/threads/off-center-steering-vgrs-fix-in-03-lx-470.1301356/) |

### 2.4. Air Suspension / Height Control (AHC)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 2.12 | Height Control Neutral Position Calibration | *Chassis → Air Suspension → Utility → Height Offset* | [Toyota TSB MC-10159708-9999 (PDF, LS500)](https://static.nhtsa.gov/odi/tsbs/2019/MC-10159708-9999.pdf) · [Lexus Owners Club — RX300 suspension](https://www.lexusownersclub.co.uk/forum/topic/115503-rx300-suspension-problems) |

### 2.5. EPB — электрический стояночный тормоз

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 2.13 | Service Mode для замены задних колодок | *Chassis → EPB → Utility → Service Mode* | [YouCanic — EPB service mode glossary](https://www.youcanic.com/glossary/active-test/) · *(подробная статья по модели — в TIS)* |

---

## 3. Body Electrical — кузовная электроника

### 3.1. SRS — подушки безопасности

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.1 | Health Check SRS, диагностика | *Body → SRS Airbag → Trouble Codes* | [vehicleservicepros — Toyota airbag alert](https://www.vehicleservicepros.com/tsbs/article/53094168/toyota-updates-airbag-alert) |
| 3.2 | Occupant Classification Sensor (OCS) Calibration | *Body → SRS → Utility → OCS Reset* | [Toyota TSB MC-10129141-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2018/MC-10129141-9999.pdf) · [Recall RCRIT-16V215-1312 (PDF)](https://static.nhtsa.gov/odi/rcl/2016/RCRIT-16V215-1312.pdf) |
| 3.3 | Seat Weight Sensor Zero Point | *Utility → Seat Weight Sensor Zero* | [Toyota TSB MC-10129144-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2018/MC-10129144-9999.pdf) |

### 3.2. Combination Meter (щиток приборов)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.4 | Maintenance Data Reset (MAINT REQD) | *Body → Combination Meter → Utility → Maintenance Reset* | [Toyota Owners Club — Oil Maint Now](https://toyotaownersclub.com/forums/topic/69319-oil-maint-now) |
| 3.5 | Oil Maintenance Reset | *Utility → Oil Maintenance Reset* | [Toyota TSB MC-10152192-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2018/MC-10152192-9999.pdf) |

### 3.3. Smart Key / Immobilizer

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.6 | Прописка смарт-ключа (Smart Code Reset) | *Body → Smart Key → Utility → Smart Code Reset* | [Toyota TSB MC-10149214-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2016/MC-10149214-9999.pdf) · [TSB MC-10152256-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2015/MC-10152256-9999.pdf) |
| 3.7 | Smart Parameter Reset | *Utility → Smart Parameter Reset* | [Toyota TSB MC-10152256-9999 (PDF, стр. Procedure B)](https://static.nhtsa.gov/odi/tsbs/2015/MC-10152256-9999.pdf) |
| 3.8 | Forced Ignition ON | *Utility → Forced Ignition ON* | [Toyota TSB MC-10152256-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2015/MC-10152256-9999.pdf) |
| 3.9 | Immobilizer Reset (транспондерные ключи, не смарт) | *Body → Immobilizer → Utility → Code Reset* | [Toyota TSB T-SB-0043-14 (PDF, обзор)](https://static.nhtsa.gov/odi/tsbs/2014/SB-10060732-2280.pdf) · [TSB MC-10238157-9999 (PDF, что НЕ поддерживается)](https://static.nhtsa.gov/odi/tsbs/2023/MC-10238157-9999.pdf) |

### 3.4. TPMS (датчики давления в шинах)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.10 | Регистрация ID датчиков | *Chassis → Tire Pressure Monitor → Utility → ID Registration* | [Modern Tire Dealer — 2023 Tacoma TPMS](https://www.moderntiredealer.com/industry-news/service/article/55269660/tpms-tire-pressure-monitoring-system-for-toyota-tacoma) · [Toyota TSB T-SB-0084-09 (PDF)](https://attachments.priuschat.com/attachment-files/2021/12/216262_T-SB-0084-09_0.pdf) |
| 3.11 | Решение «Lost Communication with ECU» (TC+CG jumper) | — | [Toyota TSB T-SB-0084-09 (PDF)](https://attachments.priuschat.com/attachment-files/2021/12/216262_T-SB-0084-09_0.pdf) · [PriusChat — TPMS error](https://www.priuschat.com/goto/post?id=2455619) |
| 3.12 | Toyota TPMS Communication Loss | *Chassis → TPM → Diagnostics* | [vehicleservicepros — Toyota TPMS Communication Loss](https://www.vehicleservicepros.com/industry-news/service-repair/article/53093254/toyota-tpms-communication-loss-2016-12-12) |

### 3.5. Power Window / Sunroof / Power Door

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.13 | Инициализация стеклоподъёмника | *Body → Power Window → Utility → Initialization* | [Toyota Owners Club — Techstream related (общая)](https://toyotaownersclub.com/forums/topic/187925-techstream-related-question) |
| 3.14 | Инициализация люка | *Body → Sunroof → Utility → Initialization* | *(процедура в ремонтном мануале Toyota по модели)* |
| 3.15 | Инициализация боковых сдвижных дверей | *Body → Power Door → Utility → Initialization* | [Toyota TSB MC-10131726-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2018/MC-10131726-9999.pdf) |

### 3.6. Customization (индивидуальные настройки)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.16 | Автоблокировка/разблокировка дверей | *Customize → Door Lock* | [Lexus Owners Club — unlock on shift to P](https://lexusownersclub.co.uk/forum/topic/120018-setting-for-unlock-doors-when-shift-to-p-techstream) · [ClubLexus — Lexus Customize Function](https://clublexus.com/forums/sc-430/782576-lexus-customize-function.html) |
| 3.17 | DRL / авто-фары / задержка освещения | *Customize → Light Control* | [OBDII365 — Toyota customization full list (Camry 2018)](https://blog.obdii365.com/2018/09/27/toyota-techstream-customization-full-list-2018-camry/) |
| 3.18 | Ответы на кнопки ключа, зуммер, язык | *Customize → Keyless* | [ClubLexus — GX470 Techstream Customize](https://www.clublexus.com/forums/gx-1st-gen-2004-2009/720333-techstream.html) |
| 3.19 | TPMS threshold, аварийка при торможении | *Customize → Vehicle* | [OBDII365 — полный список настроек Camry](https://blog.obdii365.com/2018/09/27/toyota-techstream-customization-full-list-2018-camry/) |
| 3.20 | Выбор функций Customize — общая методика (Prius Gen III) | *Customize → Save Settings* | [PriusChat — Select Customize Functions Gen III](https://priuschat.com/goto/post?id=1892737) |

### 3.7. Lighting / AFS

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.21 | Headlight Auto-Levelling Initialization | *Body → Headlight → Utility → Levelling Init* | [Lexus Owners Club — headlight level adjustment](https://www.lexusownersclub.co.uk/forum/topic/145510-headlight-level-adjustment) · [YouCanic — headlight adaptation](https://www.youcanic.com/glossary/headlight-adaptation/) |
| 3.22 | AFS Initialization | *Body → AFS → Utility → Init* | [Lexus Owners Club — RX300 headlight adjustment](https://www.lexusownersclub.co.uk/forum/topic/106136-rx300-head-light-adjustment) |

### 3.8. Air Conditioning / Climate

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 3.23 | Servomotor Position Reset | *Body → A/C → Utility → Servomotor Reset* | [Toyota TSB MC-10164328-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2019/MC-10164328-9999.pdf) |
| 3.24 | A/C Compressor Active Test | *Active Test → A/C Clutch* | [YouCanic — active test](https://www.youcanic.com/glossary/active-test/) |

---

## 4. Hybrid (гибридные модели)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 4.1 | Battery Block Voltage Check | *Hybrid → Data List → Battery Block V01..V28* | [PriusChat — reset ABS & yellow](https://www.priuschat.com/goto/post?id=2825983) |
| 4.2 | HV Battery Fan Active Test | *Active Test → Battery Fan* | [YouCanic — active test](https://www.youcanic.com/glossary/active-test/) |
| 4.3 | MG1/MG2 Resolver Learning | *Hybrid → Utility → Resolver Learn* | [PriusChat — part 3 PDF](https://attachments.priuschat.com/attachment-files/2021/04/204186_Techstream_part_3.pdf) |
| 4.4 | Insulation Resistance Check | *Hybrid → Utility → Insulation Check* | [PriusChat — part 1 PDF](https://attachments.priuschat.com/attachment-files/2021/04/204184_Techstream_part_1.pdf) |

---

## 5. Reprogramming — прошивка ECU (CUW)

| # | Процедура | Меню | Пошаговая статья |
|---|-----------|------|------------------|
| 5.1 | ECU Flash Reprogramming (Techstream + CUW) | *Function → ECU Reprogramming* | [Toyota TSB SB-10060691-2280 (PDF)](https://static.nhtsa.gov/odi/tsbs/2014/SB-10060691-2280.pdf) · [TSB SB-10060841-2280 (PDF)](https://static.nhtsa.gov/odi/tsbs/2013/SB-10060841-2280.pdf) |
| 5.2 | Global Techstream+ (GTS+) / CUW+ | *Function → ECU Reprogramming* | [Toyota TSB MC-10150418-9999 (PDF)](https://static.nhtsa.gov/odi/tsbs/2016/MC-10150418-9999.pdf) |
| 5.3 | Security Signature и подключение DCA-8000 | — | [Scribd — Techstream ECU Flash Reprogramming](https://www.scribd.com/document/445678094/Techstream-ECU-Flash-Reprogramming-Procedure-pdf) |

---

## 6. Общая справка по интерфейсу TechStream

| Источник | Что внутри |
|----------|------------|
| [PriusChat PDF — Techstream Part 1](https://attachments.priuschat.com/attachment-files/2021/04/204184_Techstream_part_1.pdf) | Главное окно, подключение, Health Check — со скриншотами |
| [PriusChat PDF — Techstream Part 3](https://attachments.priuschat.com/attachment-files/2021/04/204186_Techstream_part_3.pdf) | Utility, Active Test, Customize — большой каталог со скриншотами |
| [Scribd — Techstream Part 2](https://www.scribd.com/document/516526338/Techstream-Part-2) | Чтение DTC, Freeze Frame, Data List — со скриншотами |
| [newhilux.net — Intro & HOW-TO](https://www.newhilux.net/phpbb/viewtopic.php?p=289699) | Пошаговая установка и первое использование |
| [OBD Advisor — Techstream Review 2026](https://obdadvisor.com/toyota-techstream/) | Общий обзор, цены на подписку TIS, альтернативы |

---

## Инструкции, подробно расписанные в этом репозитории

| # | Процедура | Файл |
|---|-----------|------|
| 01 | Установка TechStream + MINI VCI | [docs/guides/01-install-techstream.md](docs/guides/01-install-techstream.md) |
| 02 | Первое подключение к автомобилю | [docs/guides/02-connect-to-vehicle.md](docs/guides/02-connect-to-vehicle.md) |
| 03 | Чтение и сброс DTC | [docs/guides/03-read-clear-dtc.md](docs/guides/03-read-clear-dtc.md) |
| 04 | Сброс адаптации АКПП | [docs/guides/04-reset-at-adaptation.md](docs/guides/04-reset-at-adaptation.md) |
| 05 | Инициализация дроссельной заслонки | [docs/guides/05-throttle-body-init.md](docs/guides/05-throttle-body-init.md) |
| 06 | Калибровка нулевой точки датчиков | [docs/guides/06-zero-point-calibration.md](docs/guides/06-zero-point-calibration.md) |
| 07 | Прокачка тормозов (ABS Active Test) | [docs/guides/07-abs-bleeding.md](docs/guides/07-abs-bleeding.md) |
| 08 | Сброс сервисного интервала + АКБ | [docs/guides/08-service-reset-battery.md](docs/guides/08-service-reset-battery.md) |

Остальные 50+ процедур из каталога — по ссылкам в таблицах выше.
