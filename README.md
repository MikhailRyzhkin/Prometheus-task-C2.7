# Prometheus-task-C2.7.

Задание C2.7

1. Разверните Prometheus Stack через docker-compose, в котором будет:

- Prometheus;
- Grafana;
- Node Exporter;
- Blackbox Exporter;
- AlertManager.

![Screenshot_1](https://user-images.githubusercontent.com/69116076/230470993-20303843-b068-4fb9-8bb1-9b130afed552.png)

Соберите метрики с https://lms.skillfactory.ru через Blackbox, соберите метрики с вашего сервера через Node Exporter.

3. Создайте dashboard в Grafana, в котором будут отображены следующие метрики:

На вашем сервере (или локальной машине):

- время работы (Uptime);
- нагрузка на процессор (CPU) в %;
- использование памяти (RAM) в %;
- использование диска в %.

![Screenshot_5](https://user-images.githubusercontent.com/69116076/230471361-f23d576a-e10e-42ab-b735-6a37eca3b0e5.png)

На lms.skillfactory.ru:

- возвращаемый статус-код;
- задержка ответа сайта;
- срок действия сертификата.

![Screenshot_4](https://user-images.githubusercontent.com/69116076/230471398-6612ed98-6515-4044-935f-1f0e461f3a03.png)


4. Добавьте алерты в AlertManager на следующие события:

- изменился статус-код сайта lms.skillfactory.ru;
- задержка превышает 5 секунд lms.skillfactory.ru;
- сервер перезагрузился (через метрику Uptime).

В Телеграм алерты можно не отправлять. Если есть желание, в качестве дополнительного задания можно кидать их себе на почту.
