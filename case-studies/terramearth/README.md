# TerramEarth

[Описание](https://services.google.com/fh/files/blogs/master_case_study_terramearth.pdf)

## Обзор компании

TerramEarth производит тяжелое оборудование для горнодобывающей и сельскохозяйственной промышленности. В настоящее время у компании более 500 дилеров и сервисных центров в 100 странах мира. Миссия TerramEarth — создавать продукты, повышающие производительность их клиентов.

## Концепция решения

В настоящее время в эксплуатации находится 2 млн транспортных средств TerramEarth и ожидаеся 20% годовой рост. Транспортные средства собирают данные телеметрии от множества датчиков в процессе работы. Небольшая часть важных данных передается с транспортных средств в режиме реального времени для облегчения управления автопарком. Остальные данные датчиков накапливаются, сжимаются и загружаются ежедневно, когда автомобили возвращаются на базу. Каждый автомобиль обычно генерирует от 200 до 500 МБ данных в день.

## Существующее техническое решение

Инфраструктура сбора и анализа данных о транспортных средствах TerramEarth развёрнута в Google Cloud и обслуживает клиентов со всего мира. Растущий объем данных с датчиков собирается с 2-х основных производственных предприятий и отправляется в частные центры обработки данных, в которых находятся их устаревшие системы управления запасами и логистикой. Частные центры обработки данных имеют несколько сетевых соединений с Google Cloud.

Веб-интерфейс для дилеров и клиентов работает в Google Cloud и обеспечивает доступ к управлению запасами и аналитике.

## Бизнес-требования

- Обеспечить прогнозирование и обнаружение неисправностей автомобиля, а также быструю отправку запчастей в дилерские центры для своевременного ремонта, где это возможно.
- Снизить эксплуатационные расходы на облачные сервисы, учитывая сезонность.
- Увеличить скорость и повысить надежность процесса разработки.
- Повысить продуктивность удалённых разработчиков без ущерба для кода или безопасности данных.
- Создать гибкую и масштабируемую платформу для разработчиков, чтобы создавать заказные API для дилеров и партнеров.

## Технические требования

- Создать новый уровень абстракции для доступа по HTTP API к устаревшим системам, чтобы обеспечить постепенный переход в облако без нарушения работы.
- Модернизировать все конвейеры CI/CD, чтобы разработчики могли развертывать рабочие нагрузки на основе контейнеров в хорошо масштабируемых средах.
- Обеспечить разработчикам возможность проведения экспериментов без ущерба для безопасности и управления.
- Создать портал самообслуживания для внутренних и партнерских разработчиков, чтобы создавать новые проекты, запрашивать ресурсы для задач анализа данных и централизованно управлять доступом к API.
- Использовать облачные решения для управления ключами и секретами, оптимизировать доступ на основе учётных записей пользователей.
- Усовершенствовать и стандартизировать инструменты, необходимые для мониторинга и устранения неполадок приложений и сети.

## Резюме

Нашим конкурентным преимуществом всегда была клиентоориентированность, способность обеспечивать отличное обслуживание клиентов и минимизировать время простоя транспортных средств. После переноса нескольких систем в Google Cloud мы ищем новые способы предоставить нашим клиентам лучшие в своем классе онлайн-услуги по управлению автопарком и улучшить работу наших дилерских центров. Наш 5-летний стратегический план заключается в создании партнерской экосистемы новых продуктов путем предоставления доступа к нашим данным, расширения возможностей автономной работы наших транспортных средств и создания пути для переноса оставшихся устаревших систем в облако.
