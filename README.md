# ДЗ 4: counter в Kubernetes

Все команды и их вывод лежат в ноутбуке. Там для каждого задания есть решения с обоснованием, логи по каждому требованию и ответы на вопросы.

## Что где лежит
- `kind-config.yaml` — кластер kind из семинара 5: 3 ноды, порты 80/443 для Ingress.
- `app/` — исходники counter-backend и counter-frontend, образы собирала сама и загружала в kind.
- `k8s/namespace.yaml` — namespace `counter` и LimitRange.
- `k8s/backend.yaml`, `k8s/frontend.yaml`, `k8s/ingress.yaml` — задание 1.
- `k8s/db.yaml` — задание 2.
- `k8s/node-exporter.yaml`, `k8s/frontend-scaler.yaml` — задание 3.
- `helm/counter/` — чарт для задания 4 и ★.

## Секреты
В репозитории нет ни сертификата, ни паролей. Сертификат выпускала через openssl в папку `certs/` (она в `.gitignore`). Пароль БД генерируется при создании Secret.

