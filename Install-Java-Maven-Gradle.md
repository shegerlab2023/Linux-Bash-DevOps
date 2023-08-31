
# Java, Maven, and Gradle Installation Guide

This README provides step-by-step instructions for installing Java, Maven, and Gradle on an Ubuntu system.

## Prerequisites

- An Ubuntu system
- Access to a terminal
- A regular user with sudo privileges

## Step 1: Installing Java

1. **Update Package Repositories:**

   Open a terminal and run the following command to update the package repositories.

   ```bash
   sudo apt update
   ```

2. **Install Default Java Development Kit (JDK):**

   Run the following command to install the default JDK:

   ```bash
   sudo apt install default-jdk
   ```

3. **Check Java Version:**

   Verify that Java has been successfully installed by checking the version:

   ```bash
   java -version
   ```

## Step 2: Installing Maven

1. **Download and Extract Maven:**

   Navigate to the official Apache Maven download page (https://maven.apache.org/download.cgi) to get the latest version's URL. Replace the URL in the following command and run it:

   ```bash
   wget -N https://dlcdn.apache.org/maven/maven-3/3.9.4/binaries/apache-maven-3.9.4-bin.tar.gz
   tar -zxvf apache-maven-*.tar.gz
   ```

2. **Move Maven to Opt Directory:**

   Move the extracted folder to the `/opt` directory:

   ```bash
   sudo mv apache-maven-<version> /opt/maven
   ```

3. **Set Up Environment Variables:**

   Open the `.bashrc` file:

   ```bash
   vi ~/.bashrc

or use vscode as we experemented in the class , type 'code .' then edit .bashrc file
   ```

   Add the following lines at the end of the file:

   ```bash
   export M2_HOME=/opt/maven
   export MAVEN_HOME=/opt/maven
   export PATH=${M2_HOME}/bin:${PATH}
   ```

   Save and exit the editor. Then, apply the changes:

   ```bash
   source ~/.bashrc
   ```

4. **Check Maven Version:**

   Verify that Maven has been successfully installed:

   ```bash
   mvn -version
   ```

## Step 3: Installing Gradle

1. **Install Gradle:**

   Run the following command to install Gradle:

   ```bash
   sudo apt install gradle
   ```

2. **Check Gradle Version:**

   Verify that Gradle has been successfully installed:

   ```bash
   gradle -v
   ```

## Conclusion

You've successfully installed Java, Maven, and Gradle on your Ubuntu system. You're now ready to develop and build Java projects using these tools.

Happy coding!
```
