Практическая работа №4 
Выполнили: Бисеров Павел, Иванов Кирилл, Луцюк Владислав 
Группа:9СА-321

2 Лабораторная работа №2. Базовая настройка IP-телефонов в среде Cisco Packet Tracer

<img width="449" height="329" alt="image" src="https://github.com/user-attachments/assets/60d0fa26-723e-47e5-8fe9-09b27b3cef3e" />

Собрали топологию

<img width="404" height="228" alt="image" src="https://github.com/user-attachments/assets/1ebd6cf3-15e6-4000-84a1-8821e4ec1565" />

Подключили телефон

<img width="624" height="249" alt="image" src="https://github.com/user-attachments/assets/b5590373-f743-42c2-94e7-2cfc28fc1d77" />

Настройка fa0/0 на CMERouter

<img width="568" height="205" alt="image" src="https://github.com/user-attachments/assets/7f8d5731-80fc-4dd9-9ded-249c5432ab98" />

Настройка dhcp и callmanager express

<img width="402" height="82" alt="image" src="https://github.com/user-attachments/assets/58ad3d20-7c94-4491-9a28-9d09c8408bfe" />

Настройка коммутатора

<img width="624" height="240" alt="image" src="https://github.com/user-attachments/assets/85ea8041-3bf2-4011-a56a-a1e0fe1eaf77" />

Раздача номеров телефонам

<img width="616" height="377" alt="image" src="https://github.com/user-attachments/assets/8d897ba0-712d-45be-b7cf-814789ee725f" />

Все работает

3 Лабораторная работа №3. Настройка конфигурации Cisco CallManager Express на маршрутизаторе Cisco 2811

<img width="416" height="310" alt="image" src="https://github.com/user-attachments/assets/286330a7-7eb6-406e-b324-50428630e107" />

Топология

<img width="463" height="287" alt="image" src="https://github.com/user-attachments/assets/358efee5-7aba-48b1-a933-d9c14df41d7f" />

Пароли

<img width="612" height="229" alt="image" src="https://github.com/user-attachments/assets/de5c1993-86d1-415f-a9d1-66425bc78c45" />

Конфигурация fa0/0

<img width="447" height="137" alt="image" src="https://github.com/user-attachments/assets/a0c054cb-ca31-4e38-a7ef-a942f0667e3d" />

Dhcp сервер

<img width="493" height="153" alt="image" src="https://github.com/user-attachments/assets/4154fd92-f63f-40eb-94e6-f74b79a60e49" />

Настройка Callmanegr express

<img width="357" height="55" alt="image" src="https://github.com/user-attachments/assets/ab50f9f5-4952-492d-aad8-9f10010ba603" />

SwitchA

<img width="624" height="397" alt="image" src="https://github.com/user-attachments/assets/04f86cd9-22c0-4849-ba6a-bbbbb6be4cd4" />

Раздача номеров

Ответы на вопросы:
1. SIP — протокол сигнализации для установки, изменения и завершения сессий VoIP (порт 5060, работает с RTP для голоса).

2. Voice VLAN — создаётся командой vlan 10, затем на порту: switchport voice vlan 10. Отделяет голосовой трафик от данных.

3. Cisco Call Manager (CUCM) — централизованная IP-АТС для крупных предприятий, работает на отдельном сервере, веб-интерфейс.

4. Cisco Call Manager Express (CME) — IP-АТС для малого бизнеса, встроена в маршрутизатор Cisco, настройка через CLI.

5. Отличие — CUCM: сервер, тысячи телефонов, GUI; CME: внутри маршрутизатора, до 240 телефонов, CLI.

6. Spanning-tree portfast — переводит порт в режим Forwarding сразу (без прослушивания STP), ускоряя подключение конечного устройства.

7. Требования к сети для голоса — низкая задержка (<150 мс), низкий джиттер, отсутствие потерь пакетов (<1%), отдельный VLAN, QoS.

8. Основные команды DHCP на маршрутизаторе Cisco:
ip dhcp pool NAME  
network 192.168.1.0 255.255.255.0  
default-router 192.168.1.1  
dns-server 8.8.8.8

4 Лабораторная работа №4. Конфигурация VOIP в среде Cisco Packet Tracer

<img width="441" height="354" alt="image" src="https://github.com/user-attachments/assets/3bddee4f-f405-4015-8154-68c7274e4a43" />

<img width="390" height="162" alt="image" src="https://github.com/user-attachments/assets/ca3b366c-4ad0-4d62-8ab4-73d3717da3b2" />

Создание и настройка VLAN

<img width="624" height="664" alt="image" src="https://github.com/user-attachments/assets/50743518-af9b-47c2-ac5f-6bf6a43b09ee" />

Включаем fa0/0 и создаем лог. подинтерфейс для vlan 10, 20, 99

<img width="606" height="283" alt="image" src="https://github.com/user-attachments/assets/3d347b0c-025b-4ac3-bed0-a0a60e29634f" />

Настройка dhcp для передачи голоса

<img width="419" height="450" alt="image" src="https://github.com/user-attachments/assets/8fa43fbc-cb66-4f54-9dd8-79f0b4d304c6" />

настройка айпи телеофнов

Контрольные вопросы:

1. SIP-телефоны – устройства или софт, использующие протокол SIP для звонков через IP-сеть.

2. Voice over IP (VoIP) – технология передачи голоса по IP-сетям (Интернет, LAN).

3. VoIP: голос поверх IP, альтернатива традиционной телефонии.

4. Хороший источник о VoIP – книги Cisco Press, документация Cisco, сайты (VoIP-info.org, Habr), курсы CCNA Collaboration.

5. IP-телефон – телефон, работающий через Ethernet/Wi-Fi, использующий IP-протоколы (SIP, H.323, Skinny).

6. IP-телефония – система связи, где голос передаётся пакетами по IP-сетям (частным или Интернет).

7. VoIP-телефон – синоним IP-телефона, работающий по технологии VoIP.

8. Маршрут по умолчанию (default route) создаётся командой:
ip route 0.0.0.0 0.0.0.0 <next-hop-IP>  

7 Лабораторная работа №7. Построение сети IP-телефонии между удаленными маршрутизаторами в среде Cisco Packet Tracer

<img width="806" height="411" alt="image" src="https://github.com/user-attachments/assets/aed9d3ad-57a1-47a3-b32c-8d8b75c0a950" />

Топология

<img width="246" height="33" alt="image" src="https://github.com/user-attachments/assets/8d6623f3-fa14-470c-aed8-652256327e57" />
<img width="233" height="30" alt="image" src="https://github.com/user-attachments/assets/32e647f8-8d68-4091-83de-58fbfc4d7993" />

хостнеймы для роутеров

<img width="612" height="124" alt="image" src="https://github.com/user-attachments/assets/dc79caa9-52b2-4899-8b3a-a8b2cbfa9fa0" />
<img width="412" height="62" alt="image" src="https://github.com/user-attachments/assets/52cc29b0-f6f6-41fd-bfb6-54cbf71f5124" />

IP адреса для роутеров

<img width="442" height="116" alt="image" src="https://github.com/user-attachments/assets/870e3092-ca8d-4a18-9973-ebf4610885c4" />
<img width="453" height="114" alt="image" src="https://github.com/user-attachments/assets/9bcf5c7c-a13f-4165-91e9-064ef3e37a29" />

Настройка интерфейса s0/3/0 на RouterA, B

<img width="402" height="60" alt="image" src="https://github.com/user-attachments/assets/449b86ff-6a0a-4ce4-af6c-628e34fef4b8" />
<img width="411" height="74" alt="image" src="https://github.com/user-attachments/assets/1a54d361-1988-464a-8231-9a4173940daf" />

Dhcp серверы

<img width="318" height="60" alt="image" src="https://github.com/user-attachments/assets/3ca27999-39e9-495a-8392-7a9a72e51d78" />
<img width="308" height="59" alt="image" src="https://github.com/user-attachments/assets/de47373c-c858-4b65-b671-cc50696f1f26" />

Настройка динамической маршрутизации на основе протокола RIP

<img width="478" height="84" alt="image" src="https://github.com/user-attachments/assets/98420c05-1434-4c61-9ff5-f705735cabef" />
<img width="456" height="88" alt="image" src="https://github.com/user-attachments/assets/2425bda4-330b-454e-bce8-b1dcb4be53c2" />

CallManager Express

<img width="364" height="49" alt="image" src="https://github.com/user-attachments/assets/41a8e324-e11e-4172-a2d5-2db0b8e7afed" />
<img width="352" height="47" alt="image" src="https://github.com/user-attachments/assets/58430933-d0ca-4b1f-80f2-6e29ee6603d4" />

Назначение диапазонов портов на Свитч A и B

<img width="622" height="254" alt="image" src="https://github.com/user-attachments/assets/7e16a88b-f02b-48e8-8d4b-4be1a3d71ab3" />
<img width="627" height="254" alt="image" src="https://github.com/user-attachments/assets/3cc38bd2-43ab-4d18-b296-b70195631fa4" />

Раздача номеров

<img width="385" height="45" alt="image" src="https://github.com/user-attachments/assets/231cdc45-6777-4d05-9f71-0ef76e0d9ee0" />
<img width="398" height="48" alt="image" src="https://github.com/user-attachments/assets/8ba91b99-b27f-457e-ad0e-90bae72e2084" />

Настройка IP-телефонов

<img width="384" height="184" alt="image" src="https://github.com/user-attachments/assets/aaff7f96-f818-4af1-bccb-4564917f1dea" />
<img width="692" height="264" alt="image" src="https://github.com/user-attachments/assets/408f470d-d7c7-48b0-ab71-9b1839363480" />

Все работает

Контрольные вопросы:

1. Маршрутизируемые протоколы (IP, IPX) — передают данные между сетями.
Протоколы маршрутизации (RIP, OSPF, EIGRP) — обмениваются маршрутной информацией между маршрутизаторами.

2. RIP (дистанционно-векторный, макс. 15 хопов).
Механизмы от петель: split horizon (не отправлять маршрут туда, откуда узнал), poison reverse (отправлять маршрут с метрикой 16), лимит хопов (16 = недоступен).
RIP vs IGRP: RIP – простой, макс. 15 хопов, IGRP – Cisco, учитывает пропускную способность, большую сеть.

3. Настройка DHCP-сервера на маршрутизаторе Cisco:
ip dhcp pool NAME
network 192.168.1.0 255.255.255.0
default-router 192.168.1.1
dns-server 8.8.8.8
exit
ip dhcp excluded-address 192.168.1.1

4. Последовательное соединение между маршрутизаторами — через интерфейсы Serial (V.35, T1/E1, etc.), используется в WAN, требует инкапсуляции (HDLC, PPP, Frame Relay).

5. Скорости Serial: от 56 кбит/с до 1.544 Мбит/с (T1), до 44.736 Мбит/с (T3). В Cisco Packet Tracer — обычно до 2 Мбит/с.

6. Минимум для VoIP: ~100 кбит/с на звонок (кодек G.711 — 64 кбит/с + 20-40 кбит/с накладные расходы). Для хорошего QoS — от 128 кбит/с на канал.

7. Выход в PSTN через IP-телефон: IP-телефон через SIP-шлюз или Cisco CME/CUCM маршрутизирует вызов на FXO-порт маршрутизатора, подключённый к городской линии.

8. Команда присвоения номера телефону (в Cisco CME, на маршрутизаторе):
ephone-dn 1
number 101

8 Лабораторная работа №8. Построение сети IP-телефонии между удаленными маршрутизаторами

<img width="1541" height="966" alt="image" src="https://github.com/user-attachments/assets/16ff6fa4-aed6-4b37-9191-96e22262153c" />

Топология

<img width="403" height="79" alt="image" src="https://github.com/user-attachments/assets/99bd7d0c-ad89-42f3-a42a-a6a473e13a15" />

Интерфейс s0/3/0

<img width="346" height="66" alt="image" src="https://github.com/user-attachments/assets/647e0e85-fdfc-44fb-846d-01521d9ab4bf" />

Eigrp маршрутизация

<img width="562" height="118" alt="image" src="https://github.com/user-attachments/assets/da97aa81-bcfe-4878-81a1-ab2e5f88c5e3" />

Пинг

<img width="431" height="102" alt="image" src="https://github.com/user-attachments/assets/90814e59-2b5d-4531-ab67-5b8c54634aac" />

FastEthernet на remoterouter

<img width="636" height="186" alt="image" src="https://github.com/user-attachments/assets/036b6655-0e32-45ca-b5fa-9701693e2919" />

Fa на cmerouter

<img width="638" height="114" alt="image" src="https://github.com/user-attachments/assets/04d48306-b188-487d-ba64-df53bb533758" />

Eigrp на remoterouter

<img width="331" height="151" alt="image" src="https://github.com/user-attachments/assets/e89f1f84-4de8-42b2-a417-b73d56162f0b" />

пароли

<img width="651" height="244" alt="image" src="https://github.com/user-attachments/assets/52b506ea-f5ad-4835-b29a-3b2dd15ef5cc" />

Транковый режим

<img width="285" height="82" alt="image" src="https://github.com/user-attachments/assets/342aea02-6c2b-4030-b914-3d42682fcbd5" />
<img width="534" height="158" alt="image" src="https://github.com/user-attachments/assets/47c10f57-d6c9-4632-967b-c44e0085dc76" />

Настройка портов в соответствии vlan

<img width="621" height="226" alt="image" src="https://github.com/user-attachments/assets/4e62180d-fa14-4591-b37d-78f38c35dde5" />
<img width="550" height="341" alt="image" src="https://github.com/user-attachments/assets/db7518c0-9db4-48b2-8967-32f524b41773" />

Тоже самое на другом свиче

<img width="451" height="156" alt="image" src="https://github.com/user-attachments/assets/21a47fe1-ef58-4972-8f95-9a6f74ed8b88" />

Dhcp сервер cmerouter

<img width="453" height="76" alt="image" src="https://github.com/user-attachments/assets/7db271f5-062b-49f3-966d-1a9d7fddcf31" />

CallManager Express

<img width="635" height="166" alt="image" src="https://github.com/user-attachments/assets/8dd71871-e770-4daa-8313-13166e42ce5e" />

Номера

<img width="458" height="63" alt="image" src="https://github.com/user-attachments/assets/9cfc1423-3646-4cdb-9d80-d272fb779538" />

<img width="454" height="154" alt="image" src="https://github.com/user-attachments/assets/1ac81659-6396-478b-8d5e-67f655dc4516" />

<img width="481" height="78" alt="image" src="https://github.com/user-attachments/assets/2c1c166b-fcd2-48f5-ab01-88386a9c0e41" />

<img width="633" height="138" alt="image" src="https://github.com/user-attachments/assets/4210c7e3-eac0-4dd9-b91c-186bf07fc15d" />

<img width="2103" height="702" alt="image" src="https://github.com/user-attachments/assets/a8461664-6679-4acb-83ec-18c1213b5c72" />

<img width="1395" height="698" alt="image" src="https://github.com/user-attachments/assets/23ff9f12-67e9-41d7-bf96-6fbc5ee5ba99" />

<img width="1397" height="704" alt="image" src="https://github.com/user-attachments/assets/77df3b06-d67b-4d0d-a325-5ef728754ca1" />

Ответы нв вопросы:

1. Последовательное соединение между маршрутизаторами – физический WAN-линк (интерфейсы Serial, V.35, X.21, EIA/TIA-232). Работает побитно по одному каналу, требует синхронизации (DCE/DTE) и инкапсуляции (HDLC, PPP, Frame Relay).

2. Скорости последовательного соединения – от 56 кбит/с до 1.544 Мбит/с (T1/DS1), 2.048 Мбит/с (E1), до 44.736 Мбит/с (T3/DS3) и выше.

3. Минимальная скорость для качества VoIP – около 100–128 кбит/с на одно звонок (G.711 кодирование 64 кбит/с + IP/UDP/RTP заголовки ~40 кбит/с). Рекомендуется от 128 кбит/с для одного вызова с запасом.

4. LDP (Label Distribution Protocol) – протокол MPLS: распространяет метки между маршрутизаторами LSR, чтобы построить пути LSP для быстрой коммутации пакетов.

5.Уровни архитектуры IP-телефонии (по модели Cisco):
Уровень 1 – абонентские устройства (IP-телефоны, софтфоны)
Уровень 2 – доступ (коммутаторы, PoE, VLAN)
Уровень 3 – сеть передачи (маршрутизация, QoS, MPLS)
Уровень 4 – управление вызовами (CUCM, CME, SIP-прокси)
Уровень 5 – приложения (голосовая почта, конференции, IVR)

6. Выход в PSTN через IP-телефон – маршрутизатор с FXO-портом или SIP-шлюз соединяется с городской АТС. IP-телефон отправляет вызов через Call Manager (CME/CUCM), который перенаправляет его на FXO или шлюз.

7. Перевод звонка & конференция:
Перевод: телефон A связывается с B, затем по SIP REFER или через Call Manager соединяет B с C, а сам выходит.
Конференция: один телефон (или сервер) смешивает аудиопотоки (mixer). При вызове третьего участника медиа смешивается центрально или в режиме Ad Hoc.

8. Перехват звонка (Call Pickup) – группа телефонов настроена на одну группу перехвата. Когда звонит один из них, другой набирает *код перехвата (например, *8), и Call Manager переадресует вызов на его телефон.


