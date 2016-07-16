# Описание
Файл *Template HW HP2530.xml* содержит темплейт *Template HW HP2530*, который состоит в группах *Templates*, *Templates Hardware* и *Templates Custom*. 
И предназначен для мониторинга коммутаторов серии HP2530 по протоколу SNMP.

*Template HW HP2530* осуществляет мониторинг:
- счетчиков интерфойсов;
- времени работы;
- датчиков работоспособности(по температуре, БП, вентиляторов);
- использование памяти;
- использование ЦПУ
- Серийного номера, версии прошивки.

## Макросы

При использовании данного темплейта рекомендуется глобально установить макрос
```text
{$SNMP_COMMUNITY}	⇒	community_name
```

# Установка
## Настройка
Включите поддержку SNMP на коммутаторе:
- Подключитесь к коммутатору
- Перейдите *System->SNMP*
- Нажмите *change*:
- Укажите *Community Name*: Ваше название коммунити
- Нажмите *Save*

## Установка
Добавьте хост в темплейт *Template HW HP2530*