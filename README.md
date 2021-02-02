# Java

## Installation in Ubuntu

> Ubuntu 20.04 LTS ( Groovy grorilla)



### Installing the [Default OpenJDK](https://packages.ubuntu.com/groovy/default-jdk) (Java 11)

At the time of writing, the lastest LTS version of Java is version 11.

```shell
sudo apt update
sudo apt install default-jdk
```

### Installing [OpenJDK 8](https://packages.ubuntu.com/groovy/openjdk-8-jdk)

```shell
sudo apt update
sudo apt install openjdk-8-jdk
```

### Installing [OpenJDK 14](https://packages.ubuntu.com/groovy/openjdk-14-jdk)

```shell
sudo apt update
sudo apt install openjdk-14-jdk
```

### Installing Oracle Java

Before installing Oracle Java, make sure you read the [Oracle JDK License](https://www.oracle.com/downloads/licenses/javase-license1.html). The license **permits only non- commercial **use of the software such as personal use and development use.

The following steps describe how to install Oracle Java 11:

1. Install the dependencies necessary to [add a new repository:](https://linuxize.com/post/how-to-add-apt-repository-in-ubuntu/) 

   ```shell
   sudo apt install software-properties-common
   ```

2. Enable the Linux Uprising PPA by running the following commands:

   ```shell
   sudo add-apt-repository ppa:linuxuprising/java
   ```

3. Once the repository is added, update the packages list and install the `oracle-java11-installer` package:

   ```sh
   sudo apt update
   sudo apt install oracle-java11-installer
   ```

## Set the Default Java Version

To check the default Java version:

```shell
java --version
```

If you have multiple Java installations to change the default version:

```shell
sudo update-alternatives --config java
```

## Set the JAVA_HOME environment variable

Some applications written in Java are using the `JAVA_HOME` environment variable to determine the Java installation location.

To set example:

```shell
export JAVA_HOME="/usr/lib/jvm/java-11-openjdk-amd64"
```

