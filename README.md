# Inception-of-Things (IoT)

## Overview
An extended École 42 project focusing on modern Infrastructure as Code (IaC) and GitOps practices. This repository demonstrates the automated provisioning of lightweight Kubernetes clusters and the implementation of a continuous delivery pipeline.

## Repository Branches
To explore different architectural approaches, this project is split into distinct branches:
* **`42` (Classic):** The strict baseline implementation required for the standard École 42 evaluation.
* **`cloud` (Advanced - *Upcoming*):** An extended environment pushing beyond the mandatory scope to experiment with enterprise-grade tools like Terraform and additional cloud technologies.

## Tech Stack
* **Provisioning & IaC:** Terraform, Ansible, Vagrant, Linux (Ubuntu)
* **Containerization & Orchestration:** Docker, Kubernetes (K3s, K3d)
* **CI/CD (GitOps):** Argo CD, GitHub



<!-- # Manual Setup: Vagrant & KVM/Libvirt


sudo apt update
sudo apt install -y qemu-system-x86 libvirt-daemon-system
sudo usermod -aG libvirt $USER

# Add HashiCorp GPG key
curl -fsSL [https://apt.releases.hashicorp.com/gpg](https://apt.releases.hashicorp.com/gpg) | sudo tee /usr/share/keyrings/hashicorp-archive-keyring.asc

# Add HashiCorp repository
echo "deb [ signed-by=/usr/share/keyrings/hashicorp-archive-keyring.asc ] [https://apt.releases.hashicorp.com](https://apt.releases.hashicorp.com) $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list


sudo apt update
sudo apt install -y vagrant

# Install required libraries and network tools
sudo apt install -y ebtables libguestfs-tools libvirt-dev libxslt1-dev libxml2-dev zlib1g-dev ruby-dev

# Compile and install the vagrant-libvirt provider
vagrant plugin install vagrant-libvirt -->


<!-- extend default lvm disck

# Extend the logical volume to use 100% of the available free space
sudo lvextend -l +100%FREE /dev/mapper/ubuntu--vg-ubuntu--lv

# Resize the filesystem to fill the newly extended volume
sudo resize2fs /dev/mapper/ubuntu--vg-ubuntu--lv -->


<!-- Dont forget to install requirement : ansible-galaxy collection install -r confs/requirements.yml -->