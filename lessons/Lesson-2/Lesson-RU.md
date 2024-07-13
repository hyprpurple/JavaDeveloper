### 🔧 Java Development Kit (JDK)

> Перед началом изучения языка программирования Java необходимо установить Java Development Kit (JDK) — компонент,
> основной для среды разработки Java, предоставляющий все необходимые инструменты и исполняемые бинарные файлы для
> компиляции, отладки и выполнения Java-программ. [Скачать](https://www.oracle.com/cis/java/technologies/downloads/#jdk22-windows)

---

### Установка JDK на Windows:

- Запустите установленый файл
- "Следуйте инструкциям в менеджере установки

### Установка JDK на MacOS:

- Запустите установленый файл
- "Следуйте инструкциям в менеджере установки

### Установка JDK на Linux:

- Распакуйте архив с помощью команды `tar`: 

    ```bash
    tar -xzf jdk-VERSION-linux-x64.tar.gz
    ```
- Можно переместить распакованный JDK в нужное место, например, в `/usr/lib/jvm/`:

    ```bash
    sudo mkdir -p /usr/lib/jvm
    ```

    ```bash
    sudo mv jdk-VERSION-linux-x64 /usr/lib/jvm/
    ```
  
- Добавьте переменную окружения `JAVA_HOME` в ваш файл `.bashrc`:

    ```bash
    export JAVA_HOME=/usr/lib/jvm/jdk-VERSION
    ```

- Сохраните файл `.bashrc` и загрузите изменения:

    ```bash
    source ~/.bashrc
    ```

- Добавьте путь к bin директории JDK в переменную PATH, чтобы можно было использовать Java и другие инструменты JDK
  из любого места в системе:

    ```bash
    export PATH=$JAVA_HOME/bin:$PATH
    ```

- Проверьте установку JDK, выполните:

    ```bash
    java -version
    ```
