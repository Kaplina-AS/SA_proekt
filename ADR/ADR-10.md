# ADR-10: Выбор языка программирования для микросервисов 

### Статус

Предложено (зависит от сервиса)

### Контекст

- Различные микросервисы могут иметь разные требования к производительности, масштабируемости, скорости разработки и доступности библиотек.
- Необходимо использовать оптимальный язык программирования для каждой задачи.
- Необходимо учитывать опыт и экспертизу команды.
- Рассматривались альтернативные стратегии (использование одного языка для всех сервисов), но использование разных языков было выбрано для обеспечения большей гибкости и оптимизации.

### Решение

- Использовать разные языки программирования в зависимости от сервиса (Polyglot Persistence).
- Рекомендуемые языки:
+ Auth Service: Java (Spring Boot) или Python (Django/Flask)
+ User Profiles Service: Java (Spring Boot) или Node.js (Express)
+ Workout Service: Java (Spring Boot) или Go
+ Fitness Trackers Service: Node.js (Express) или Python (Flask)
+ Recommendation Service: Python (Scikit-learn, TensorFlow)
+ Payment Service: Java (Spring Boot)
+ Notification Service: Node.js (Express)
- Обеспечить согласованность в стиле кодирования и документировании.

### Последствия

(+) Возможность выбора наилучшего инструмента для каждой задачи.

(+) Гибкость в использовании различных технологий.

(-) Потенциальное увеличение сложности поддержки и экспертизы команды.