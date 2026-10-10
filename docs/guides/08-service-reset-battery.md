# 08. Сброс сервисного интервала и регистрация АКБ

Два разных действия, которые часто нужны вместе после планового ТО:
1. Погасить лампу **MAINT REQD** / значок ключа.
2. Сообщить блоку управления, что установлен **новый** аккумулятор (на моделях с системой контроля заряда).

---

## Часть A. Сброс сервисного интервала

### Способ 1. Без TechStream

На большинстве Toyota работает так:

1. Выключите зажигание.
2. Нажмите и удерживайте кнопку **Trip/Odo** (сброс пробега).
3. Включите зажигание **IG-ON** (не запуская двигатель), продолжая держать кнопку.
4. На щитке появляется счётчик моточасов, затем надпись меняется с `------` на `000000`.
5. Отпустите кнопку, выключите зажигание.

![Кнопка Trip/Odo](images/08-service-01-trip-button.png)

Если способ не сработал — используйте TechStream.

### Способ 2. Через TechStream

1. [Подключитесь к автомобилю](02-connect-to-vehicle.md).
2. **System Select** → **Body Electrical** → **Combination Meter** (комбинация приборов).
3. Вкладка **Utility** → **Maintenance Data Reset** / **Oil Maintenance Reset**.
4. **Next** → подтвердите → *«Reset completed»*.

![Maintenance Data Reset](images/08-service-02-maint-reset.png)

5. Выключите зажигание на 10 секунд. Проверьте, что сервисная лампа погасла.

---

## Часть B. Регистрация нового аккумулятора

> 💡 Полная регистрация АКБ в стиле BMW/Mercedes на обычных Toyota **не требуется**. Но на моделях с **Battery Management System** (Prius, гибриды, Lexus с системой Charging Control) нужно сбросить статистику разряда/заряда.

### Шаг 1. Проверьте необходимость

В **Data List → Engine** посмотрите параметры:

- **Battery SOC (State of Charge) %** — текущий заряд.
- **Charge Control Target Voltage** — целевое напряжение.
- **Battery Current Integration** — интеграл тока.

Если есть **Battery Current Integration** — значит, ECU ведёт историю, которую нужно сбросить после замены.

![Параметры АКБ в Data List](images/08-service-03-battery-data.png)

### Шаг 2. Сброс через Utility

1. **System Select** → **Engine and ECT**.
2. **Utility** → **Battery Reset** / **Current Sensor Learning Value Clear**.
3. **Next** → подтвердите.
4. Дождитесь *«Battery Reset completed»*.

![Battery Reset](images/08-service-04-battery-reset.png)

### Шаг 3. Инициализация датчика тока

Если установлен датчик тока на минусовой клемме АКБ:

1. **Utility** → **Current Sensor Initialization**.
2. Отсоедините потребители (фары, печку, аудио).
3. Нажмите **Start**, подождите ~30 секунд.

![Инициализация датчика тока](images/08-service-05-current-sensor.png)

### Шаг 4. Для гибридов

Для Prius/Camry Hybrid и т.п. **12-вольтовый** вспомогательный АКБ сбрасывается так же, но **тяговый** аккумулятор не трогается — его параметры контролирует отдельный HV ECU, обычное обслуживание в TechStream не требуется.

Если нужно посмотреть состояние тяговой батареи:
**System Select → Hybrid Control → Data List → Battery Block Voltage V01…V14 (или V28)** — разброс между блоками не должен превышать **0.2 В**.

![Battery Block Voltage](images/08-service-06-hv-blocks.png)

---

## Проверка результата

После сброса и короткой поездки (20–30 мин):

- **Battery SOC** должен постепенно подняться к 80–90%.
- **Charge Control** работает — напряжение на АКБ меняется (13.2 ↔ 14.6 В) в зависимости от нагрузки, это нормально.
- Сервисная лампа и значок АКБ погашены.

---

## Источники со скриншотами

- [Toyota Owners Club — Maintenance Reset discussion](https://toyotaownersclub.com/forums/topic/187925-techstream-related-question) — как сбросить MAINT REQD через Combination Meter → Utility.
- [PriusChat — Reset ABS light & yellow (!)](https://www.priuschat.com/goto/post?id=2825983) — сбросы после работ с АКБ и инициализация датчика тока.

**Все инструкции:** [← вернуться к оглавлению](../../README.md)
