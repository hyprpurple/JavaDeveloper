### 🔧 Java Development Kit (JDK)

> Before starting to learn the Java programming language, you need to install the Java Development Kit (JDK) — the core
> component for Java development environment, providing all necessary tools and executable binaries for compiling,
> debugging, and running Java programs. [Download](https://www.oracle.com/cis/java/technologies/downloads/#jdk22-windows)

---

### Installing JDK on Windows:

- Run the downloaded file.
- Follow the instructions in the installation wizard.

---

### Installing JDK on MacOS:

- Run the downloaded file.
- Follow the instructions in the installation wizard.

---

### Installing JDK on Linux:

- Extract the archive using the tar command:

    ```bash
    tar -xzf jdk-VERSION-linux-x64.tar.gz
    ```
- Move the unpacked JDK to the desired location, for example, `/usr/lib/jvm/`:
- 
    ```bash
    sudo mkdir -p /usr/lib/jvm
    ```

    ```bash
    sudo mv jdk-VERSION-linux-x64 /usr/lib/jvm/
    ```
  
- Add the `JAVA_HOME` environment variable to your `.bashrc` file:

    ```bash
    export JAVA_HOME=/usr/lib/jvm/jdk-VERSION
    ```

- Save the `.bashrc` file and load the changes:

    ```bash
    source ~/.bashrc
    ```

- Add the JDK `bin` directory to your PATH variable to use Java and other JDK tools from anywhere in the system:

    ```bash
    export PATH=$JAVA_HOME/bin:$PATH
    ```

- Verify the JDK installation:

    ```bash
    java -version
    ```
