# Система журналирования в операционных системах Linux
Система журналирования в операционных системах Linux работает на базе демона journald, который занимается обработкой сообщений от служб, initrd, ядра и т.д. Доступ к собранной в журнале информации осуществляется путем использования утилиты journalctl. Она же дает возможности для управления: делать фильтрацию, менять формат отображения, мониторить активные процессы и пр.

Основная задача журнальной системы systemd — централизация управления собираемыми данными независимо от источника. При помощи демона journald система объединит информацию в двоичном формате. Это позволяет повысить гибкость настройки и одинаково легко работать с задачами любой сложности. Например, комбинировать записи нескольких служб для выявления общей проблемы.

Система журналирования systemd универсальная. Ее применяют вместе с действующей syslog, вместо syslog и в качестве дополнения активных механизмов заполнения журнала. Допускается и объединение технологий, если этого требует выполнение конкретных задач.

# timedatectl list-timezones
 <img width="285" height="355" alt="image" src="https://github.com/user-attachments/assets/1c156ddb-6358-453f-80f5-80744d6c06fe" />

# sudo timedatectl set-timezone zone
<img width="498" height="161" alt="image" src="https://github.com/user-attachments/assets/babf0705-691c-4c87-a7aa-834bbd021a18" />

# timedatectl status
<img width="413" height="129" alt="image" src="https://github.com/user-attachments/assets/f74f8911-b367-4d8e-867d-e0597c7fe650" />

# journalctl
<img width="640" height="186" alt="image" src="https://github.com/user-attachments/assets/4d4173d7-dcce-4c2b-a517-e247eb025342" />
# journalctl –utc
<img width="207" height="45" alt="image" src="https://github.com/user-attachments/assets/6751b710-f11d-469d-94ea-a9fdb45b399f" />

# journalctl –b
<img width="533" height="183" alt="image" src="https://github.com/user-attachments/assets/547e984a-f023-4228-a87b-20f700340a29" />

# -- Reboot --
