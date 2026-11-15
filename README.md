# Настройка SSH-доступа к GitHub

## 1. Установка SSH-клиента и генерация ключевой пары

### Проверка версии SSH
```bash
ssh -V
```

### Генерация ключа
```bash
ssh-keygen -t ed25519 -C "antonzaxarow2004@gmail.com"
```

### Проверка файлов
```bash
ls -la ~/.ssh/
```

### Публичный ключ
```bash
cat ~/.ssh/id_ed25519.pub
```

### Вывод
![ssh-keygen](screen/keygen.png)
![lsSSH](screen/lsSSH.png)
![pubKey](screen/pubKey.png)


## 2. Добавление публичного ключа в GitHub

### Вывод
![pubKey](screen/pubKeygit.png)

## 3. Проверка SSH-подключения

```bash
ssh -T git@github.com
```

### Вывод
![test](screen/test.png)

## 4. Клонирование

```bash
git clone git@github.com:ZakharovAntonYY/hm_3.git
```

### Вывод
![clone](screen/gitClone.png)

## 5. Коммит и push

```bash
git add -A
git commit -m "add doc"
git push origin main
```

### Вывод
![push](screen/gitPush.png)

