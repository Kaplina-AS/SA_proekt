# ADR-08: Выбор системы оркестрации контейнеров: Kubernetes

### Статус

Предложено (требует дальнейшей оценки)

### Контекст

- Необходимо автоматизировать развертывание, масштабирование и управление контейнерами.
- Необходимо обеспечить отказоустойчивость и автоматическое восстановление сервисов.
- Необходимо упростить процесс обновления и отката версий микросервисов.
- Требуется возможность мониторинга и логирования контейнеров.
- Рассматривались альтернативные решения (Docker Swarm, AWS ECS), но Kubernetes был выбран из-за его широкой поддержки, развитой экосистемы и большого сообщества.

### Решение

- Рассмотреть Kubernetes для оркестрации контейнеров.
- Определить стандартизованные конфигурации Kubernetes для развертывания микросервисов.
- Использовать Helm для управления конфигурациями Kubernetes.
- Настроить мониторинг и логирование Kubernetes.
- Провести обучение команды Kubernetes.

### Последствия

(+) Автоматизация развертывания и масштабирования.

(+) Отказоустойчивость и автоматическое восстановление сервисов.

(-) Сложность настройки и управления.

(-) Требует значительных знаний и опыта.

### Альтернативы

Docker Swarm, AWS ECS