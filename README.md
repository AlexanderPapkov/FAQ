# FAQ

## Заметки по Docker 

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
