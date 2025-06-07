# Cluster Docker Swarm com Vagrant

Este projeto configura automaticamente um cluster **Docker Swarm** usando **Vagrant** e **VirtualBox**. Ele cria 4 máquinas virtuais Ubuntu com Docker instalado:

- `master` (manager do cluster)
- `node01`, `node02` (workers)

## 📦 Estrutura do Projeto
vagrant-docker-swarm/
├── Vagrantfile
├── docker.sh # Instala Docker
├── master.sh # Inicializa o Swarm

## 🚀 Requisitos

- [Vagrant](https://www.vagrantup.com/)
- [VirtualBox](https://www.virtualbox.org/)
- Acesso a internet para instalar pacotes nas VMs

## ⚙️ Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/vagrant-docker-swarm.git
cd vagrant-docker-swarm

vagrant up

vagrant ssh master

docker node ls

🛑 Como Derrubar o Ambiente

vagrant destroy -f




