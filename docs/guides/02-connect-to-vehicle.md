# 02. Первое подключение к автомобилю

**Время выполнения:** 5 минут.
**Требуется:** установленный TechStream (см. [инструкцию 01](01-install-techstream.md)), кабель MINI VCI.

---

## Правильная последовательность подключения

> 💡 Это важно: нарушение порядка — частая причина ошибки *«No communication with ECU»*.

1. **TechStream пока НЕ запускать.**
2. Подключите MINI VCI в USB-порт ноутбука.
3. Запустите TechStream двойным кликом по ярлыку.
4. **Теперь** подключите OBD-разъём кабеля в автомобиль.
5. Поверните ключ зажигания в положение **IG-ON** (вторая позиция, без запуска двигателя).

![Разъём OBD-II под рулевой колонкой](images/02-connect-01-obd-port.svg)

## Шаг 1. Запуск сессии

На главном экране TechStream нажмите **Connect to Vehicle** (большая кнопка слева).

![Главное меню Connect to Vehicle](images/02-connect-02-main-menu.svg)

## Шаг 2. Выбор модели и года

Программа попытается определить VIN автоматически. Если не удалось — укажите вручную:

- **Division:** Toyota / Lexus / Scion.
- **Model:** модель.
- **Model Year:** год выпуска (**важно**: год модельный, не календарный).
- **Engine:** код двигателя.
- **Options:** AWD / 2WD, тип трансмиссии.

![Выбор модели](images/02-connect-03-vehicle-select.png)

Нажмите **Next**.

## Шаг 3. Health Check (опционально)

Первый вопрос программы: *Perform Health Check?*
- **Yes** — быстрое сканирование всех ECU, занимает 1–3 минуты.
- **No** — переход к ручному выбору системы.

![Health Check](images/02-connect-04-health-check.png)

## Шаг 4. Главный экран диагностики

Откроется окно **System Select** со списком всех блоков управления:

- **Powertrain** — двигатель, АКПП, круиз-контроль.
- **Chassis** — ABS/VSC, рулевое, подвеска.
- **Body Electrical** — SRS (подушки), иммобилайзер, кузовная электроника.

Зелёный значок — связь установлена, серый — блок не отвечает / не установлен.

![System Select](images/02-connect-05-system-select.svg)

## Шаг 5. Безопасное отключение

1. **Pull Down** → **Exit** в меню TechStream.
2. Выключите зажигание.
3. Отсоедините OBD-разъём от автомобиля.
4. Отсоедините USB от ноутбука.

> ⚠️ Не вытаскивайте кабель во время активной сессии — можно вызвать зависание ECU.

---

## Частые ошибки подключения

| Сообщение | Причина |
|-----------|---------|
| *No communication with ECU* | Зажигание выключено, перегоревший предохранитель OBD, нарушенный порядок подключения |
| *Vehicle not supported* | Выбран неверный год/регион TechStream |
| *CAN bus error* | Проблема с проводкой CAN-шины, обрыв витой пары |

## Источники со скриншотами

- [Toyota Owners Club — «How to connect your laptop to the OBD socket»](https://toyotaownersclub.com/forums/topic/156801-how-to-connect-your-laptop-to-the-obd-socket) — фото OBD-разъёма на разных моделях и скриншоты окна подключения.
- [PriusChat — proper procedure when using MINI VCI](https://priuschat.com/goto/post?id=2160919) — правильный порядок запуска: TechStream → кабель → зажигание.
- [Toyota Owners Club — «Success with Techstream»](https://toyotaownersclub.com/forums/topic/186797-success-with-techstream) — скриншоты выбора модели, года и двигателя.

**Следующий шаг:** [03. Чтение и сброс кодов неисправностей →](03-read-clear-dtc.md)
