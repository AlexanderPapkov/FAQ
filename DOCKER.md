# FAQ

## Заметки по Docker 

### Запуск процессов Docker

Чтобы Docker запускался автоматически при загрузке системы, нужно ввести команду:

```sudo systemctl enable docker.service```

```sudo systemctl enable containerd.service```

Чтобы исключить из автоматического запуска:

```sudo systemctl disable docker.service```

```sudo systemctl disable containerd.service```

Чтобы добавить docker в группу пользователей:

```sudo groupadd docker```

Чтобы добавить текущий профиль:

```sudo usermod -aG docker $USER```

### Моменты по сборке

Dockerfile не позволяет копировать (COPY/ADD) вне директории, где он находится. Поэтому все файлы, которые находятся вне, необходимо перетащить в туже папку, где и будет проходить сборка. 

## Заметки по Docker Compose 

Он должен быть установлен в систему
