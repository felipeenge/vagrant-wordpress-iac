# Vagrant WordPress IaC Provisioning

This project is a DevOps portfolio entry that demonstrates how to automatically provision a complete LAMP (Linux, Apache, MySQL, PHP) stack using Vagrant and Shell scripting, applying **Infrastructure as Code (IaC)** concepts.

The project sets up an Ubuntu virtual machine, installs the necessary services, creates the database, and deploys a fully functional WordPress instance automatically.

---

## 🛠️ Technologies Used

- **Vagrant** (Environment Management)
- **VirtualBox** (Virtualization Provider)
- **Ubuntu 20.04 LTS** (Focal Fossa)
- **Apache2** (Web Server)
- **MySQL** (Database Server)
- **PHP 7.4+** (Server-side Scripting)
- **Shell Script** (Automated Provisioning)

---

## 🎯 Project Goals

- Practice **Infrastructure as Code (IaC)** principles.
- Automate the installation of a dynamic web environment (LAMP Stack).
- Handle database provisioning and user permissions via script.
- Automate Apache VirtualHost configuration.
- Demonstrate the transition from manual QA testing environments to automated DevOps pipelines.

---

## 📌 What This Project Does

When you run `vagrant up`, the script performs the following steps automatically:

1.  **VM Creation:** Creates an Ubuntu 20.04 VM using Vagrant.
2.  **Network Setup:** Configures a private network with a static IP.
3.  **Package Installation:** Updates the OS and installs Apache, MySQL, PHP, and required extensions.
4.  **WordPress Setup:** Downloads the latest WordPress release and sets permissions.
5.  **Server Configuration:** Configures Apache VirtualHost for the site.
6.  **Database Automation:** Creates the MySQL database, user, and grants privileges.
7.  **Config Generation:** Automatically generates the `wp-config.php` file with database credentials.

---

## 🌐 Network Configuration

- **VM Private IP:** `192.168.58.30`
- **Access the website at:** [http://192.168.58.30](http://192.168.58.30)

---

## 🚀 How to Run the Project

### Prerequisites

- [VirtualBox](https://www.virtualbox.org/wiki/Downloads) installed
- [Vagrant](https://www.vagrantup.com/downloads) installed
- Git (optional)

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/felipeenge/vagrant-wordpress-iac.git
   cd vagrant-wordpress-iac

2. Start the environment:
    ```bash
    vagrant up

3. Access the application
    ```bash
    After provisioning finishes, open your browser and go to: http://192.168.58.30

⚙️ Management Commands
- **Re-run Provisioning (if you changed the script):** 

1. Provisioning:
    ```bash
    vagrant provisioning

3. Reload the VM and provision again:
    ```bash
    vagrant reload --provision

4. Stop the Environment:
    ```bash
    vagrant halt

5. Destroy the Environment (Delete VM and data):
    ```bash
    vagrant destroy


