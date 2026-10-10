# Источники

Аннотированный список статей, форумных тем и официальных документов, на которых основаны инструкции. У большинства — живые скриншоты интерфейса TechStream и фотографии процедур.

> Открывайте оригинал по ссылке и смотрите снимки экрана в контексте авторской статьи.

---

## 01. Установка TechStream и драйверов MINI VCI

- [Drive2 — «Установка Techstream на Windows 7, 8.1, 10 — x64 bit»](https://www.drive2.ru/b/479152325051547873/)
  Пошаговая русскоязычная статья с живыми скриншотами. Разбор обходного пути для 64-битной Windows: распаковка `MVCI Driver for TOYOTA.msi` командой `msiexec /a`, ручная установка драйвера FTDI через Диспетчер устройств, выбор интерфейса «XHorse — MVCI» в настройках TechStream.
- [PriusChat — «techstream inconsistencies»](https://priuschat.com/goto/post?id=2444747)
  Обсуждение частых проблем: автоматическая установка драйвера Windows ломает COM-порт, `FirmwareUpdateTool.exe` не работает на Windows 8/10. Советы: удалить ранее установленные устройства из Диспетчера, запретить Windows автоматический поиск драйверов.
- [RTS Auto — PDF «MVCI Driver ended prematurely»](https://www.rtsauto.com/wp-content/uploads/2019/10/MVCI-Driver-ended-prematurely-error.pdf)
  Разбор ошибки инсталлятора на x64 Windows, с иллюстрациями.
- [newhilux.net — «Toyota Techstream + mini-VCI kit: Intro & HOW-TO»](https://www.newhilux.net/phpbb/viewtopic.php?p=289699)
  Англоязычный пошаговый гайд с большим количеством скриншотов главного меню, подключения и выбора ПО.

## 02. Первое подключение к автомобилю

- [Toyota Owners Club — «How to connect your laptop to the OBD socket»](https://toyotaownersclub.com/forums/topic/156801-how-to-connect-your-laptop-to-the-obd-socket)
  Инструкция с фотографиями расположения OBD-II разъёма под рулевой колонкой на разных моделях Toyota, скриншоты экрана `Vehicle Connection Wizard` и `System Select`.
- [PriusChat — Techstream connection procedure](https://priuschat.com/goto/post?id=2160919)
  Правильный порядок действий: сначала запустить TechStream, затем подключить OBD-кабель, затем включить зажигание. Разбор типовых ошибок.
- [Toyota Owners Club — «Success with Techstream»](https://toyotaownersclub.com/forums/topic/186797-success-with-techstream)
  Скриншоты окна выбора модели, года выпуска, двигателя. Что делать, если VIN не определился автоматически.

## 03. Чтение и сброс кодов неисправностей (DTC)

- [NHTSA TSB SB-10062028-2280 (Toyota)](https://static.nhtsa.gov/odi/tsbs/2013/SB-10062028-2280.pdf)
  Официальный бюллетень Toyota с иллюстрациями TechStream: `Trouble Codes`, `Freeze Frame Data`, `Clear DTC`. Как читать статус Current / Pending / History.
- [NHTSA TSB MC-10132450-9999 (Toyota iA 2016)](https://static.nhtsa.gov/odi/tsbs/2017/MC-10132450-9999.pdf)
  Какие коды нельзя очистить (U0323, U0423, U3000) и при каких условиях, требования к версии ПО (Techstream 12.10.018+).
- [Toyota Owners Club — «Techstream related question»](https://toyotaownersclub.com/forums/topic/187925-techstream-related-question)
  Нюансы отображения кодов и работы с Freeze Frame.

## 04. Сброс адаптации АКПП

- [Drive2 — заметка по сбросу адаптации Aisin AWF8](https://www.drive2.ru/l/593361071729814017/)
  Описание процедуры: прогрев ATF, Reset Memory через TechStream, цикл обкатки.
- [Drive2 — альтернативный разбор](https://www.drive2.ru/l/566077790198169720/)
  Что такое адаптация, в чём отличие Reset Memory от AT Initialization, живые фото Data List с температурой ATF.
- [Drive2 — опыт сброса на TLC Prado 150](https://www.drive2.ru/l/707437327256921961/)
  Пошагово с фотографиями ноутбука и экрана TechStream; важен прогрев коробки до 60–80 °C.
- [ClubLexus — «Techstream»](https://www.clublexus.com/forums/ls-4th-gen-2007-2017/910649-techstream.html)
  Англоязычный разбор пунктов `Utility` для АКПП: Reset Memory, AT Initialization — чем различаются.

## 05. Инициализация дроссельной заслонки

- [Toyota Owners Club — «Throttle re-learn procedure»](https://toyotaownersclub.com/forums/topic/195291-throttle-re-learn-procedure)
  Выдержка из сервисной информации Toyota: отключить минусовую клемму ≥60 сек, зажигание ON без педали, подключить TechStream и очистить DTC, прогреть двигатель с отключёнными потребителями.
- [TPautoRepair — «How do I reset the electronic throttle control»](https://tpautorepair.net/how-do-i-reset-the-electronic-throttle-control/)
  Упрощённое объяснение процедуры «идле лёрн» без диагностики, с иллюстрациями подкапотного пространства.
- [2CarPros — обсуждение P1589](https://2carpros.com/questions/acceleration-learning-value--1661232)
  Пример живого Data List: что должно показывать TPS% на закрытой/открытой заслонке.

## 06. Калибровка нулевой точки датчиков (Yaw / G / Steering Angle)

- [vehicleservicepros.com — «Toyota zero point calibration» (TSB 2014)](https://www.vehicleservicepros.com/tsbs/article/53092346/toyota-zero-point-calibration-2014-10-06)
  Переопубликованный Toyota TSB. Условия, менюшки TechStream, обязательные шаги. Иллюстрации заводского интерфейса.
- [ClubLexus — «How to do a zero point calibration via Techstream»](https://www.clublexus.com/forums/ls-3rd-gen-2001-2006/789241-how-to-do-a-zero-point-calibration-via-techstream.html)
  Подробная обсуждаемая процедура со скриншотами: Reset Memory → Test Mode → ожидание ≥ 2 сек, индикация на панели приборов.
- [PriusChat PDF — «Yaw Rate and Acceleration Zero Point» (Prius SM 250911)](https://attachments.priuschat.com/attachment-files/2024/05/250911_Prius_SM_-_Yaw_Rate_and_Acceleration_Zero_Point.pdf)
  Оригинальная страница из сервисного мануала Prius с таблицей условий и схемами.
- [PriusChat PDF — «Yaw rate sensor» (123019)](https://attachments.priuschat.com/attachment-files/2017/04/123019_Yaw_rate_sensor.pdf)
  Что проверять до калибровки, диагностика самого датчика.
- [NHTSA TSB MC-10109460-9999](https://static.nhtsa.gov/odi/tsbs/2014/MC-10109460-9999.pdf)
  Инициализация VGRS: поездка по прямой со скоростью ≥35 км/ч ≥5 секунд.

## 07. Прокачка тормозов через Active Test (ABS)

- [PriusChat — «Question about bleeding brakes with Techstream»](https://www.priuschat.com/goto/post?id=2862028)
  Разбор ошибки «air bleeding has failed», неверные подсказки в мануале Bentley по реле мотора ABS, что проверить в блоке реле.
- [ih8mud.com — «ABS bleed harness»](https://forum.ih8mud.com/threads/abs-bleed-harness.1370459/)
  Обсуждение по Land Cruiser: что умеет Active Test, что нет, когда без него не обойтись.
- [NHTSA TSB MC-10220187-9999](https://static.nhtsa.gov/odi/tsbs/2022/MC-10220187-9999.pdf)
  Пример официальной процедуры Active Test с требованиями к версии TechStream.

## 08. Сброс сервисного интервала и регистрация АКБ

- [Toyota Owners Club — тема по Maintenance Reset](https://toyotaownersclub.com/forums/topic/187925-techstream-related-question)
  Как сбросить лампу MAINT REQD через Combination Meter → Utility.
- [PriusChat — «How do you reset ABS light & yellow»](https://www.priuschat.com/goto/post?id=2825983)
  Обсуждение сбросов после работ с АКБ и инициализации датчика тока.

---

## О копировании контента

Статьи и скриншоты по ссылкам защищены авторским правом их владельцев и правами Toyota на интерфейс TechStream. Этот репозиторий **не содержит копий** защищённого контента: только ссылки, краткие пересказы процедур своими словами и собственные схемы в SVG. Если вам нужны живые скриншоты в документе — делайте их сами с лицензионной копии TechStream.
