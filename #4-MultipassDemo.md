#4 Assignment 4: Multipass Demo for Server Management
- Submit the steps here with screenshots

## 1. Multipass Installation

Multipass was installed on the Windows host system to create and manage lightweight Ubuntu virtual machine instances.

After installation, the Multipass installation was verified using the command-line interface.

![Multipass Installation](ass 4\multipass installation.png)

---

## 2. Verification of Multipass

The Multipass installation was verified to ensure that the application was installed correctly and ready to create Ubuntu instances.

The available Ubuntu images and Multipass environment were checked before launching the required instance.

![Verification of Multipass](ass 4\Verification of multipass.png)

---

## 3. Creating a Multipass Instance

A new Ubuntu Server instance was created using Multipass.

The instance was named using my name and register number.

```bash
multipass launch jammy --name prabakaran-23cb031
multipass list
multipass shell prabakaran-23cb031
```

![Launching Multipass](ass 4\Launching an multipass instance.png)

## 4. Updating the Package Repository

After entering the Ubuntu Server instance, the package repository was updated using:
```bash
sudo apt update
``` 
Updating the package repository ensures that the latest available package information is retrieved before installing new software.

5. Installing Apache Web Server

Apache2 was selected as the web server for this assignment.

It was installed using:
```bash
sudo apt install apache2 -y
sudo systemctl status apache2
```
The Apache service was then verified to ensure that the web server was running successfully.

![Updating](ass 4\Updating & installing apache.png)
![output](ass 4\OUTPUT.png)


## 6.Web Server Verification

The Apache web server was tested from inside the Multipass instance using:
```bash
curl http://localhost
```
The command successfully returned the HTML content of the Apache2 Ubuntu Default Page, confirming that the web server was running and responding correctly.

![apache](ass 4\Apache on local browser - OUTPUT.png)


