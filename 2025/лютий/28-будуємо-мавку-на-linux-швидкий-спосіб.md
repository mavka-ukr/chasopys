# Будуємо Мавку на GNU/Linux (швидкий спосіб)

Як просто і швидко збудувати <subject>Мавку</subject> на Linux? Читайте далі.

## Встановлення залежностей

Нам будуть потрібні **Clang** та **Git**.

Встановлення **Clang** та **Git** на **Ubuntu Linux**:

```shell
sudo apt install git clang
```

Встановлення **Clang** та **Git** на **Arch Linux**:

```shell
sudo pacman -S git clang
```

## Будування

Клонуємо репозиторій з підготовленими файлами:

```shell
git clone https://github.com/mavka-ukr-static/mavka-linux-x86_64 --depth=1
```

Відкриваємо клоновану теку:

```shell
cd mavka-linux-x86_64
```

Будуємо:

```shell
sh build.sh
```

Пробуємо:

```
./out/мавка
```

Для зручності, <subject>Мавку</subject> можна встановити глобально:

```shell
sudo cp ./out/мавка /usr/local/bin
```

---

Читайте також:

- [Як збудувати <subject>Мавку</subject> на Linux з джерельних файлів?](./2025-02-28-будуємо-мавку-на-linux.html)

---

_Написав [Давид](https://кдб.укр). Опубліковано 28.02.2025._