# rd-fluxcd-lesson

#### У результаті було реалізовано повний GitOps workflow за допомогою Flux CD та Kustomize. Flux CD був підключений до GitHub репозиторію та автоматично синхронізував Kubernetes кластер із manifests у Git.

#### Для застосунку simple-app було створено Kustomize base та overlays для середовищ development і production. У development було розгорнуто 1 репліку застосунку та Dragonfly instance через Operator Pattern, а у production — 3 репліки застосунку, Dragonfly з 2 репліками та HorizontalPodAutoscaler.

#### Також було перевірено механізм drift reconciliation: після ручного видалення Service Flux автоматично відновив ресурс відповідно до стану, описаного в Git репозиторії.

![alt text](<screenshots/Screenshot 2026-05-17 at 13.42.03.png>)
