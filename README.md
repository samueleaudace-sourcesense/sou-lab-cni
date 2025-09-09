
#Progetto Vagrant + Ansible
#Descrizione

Il laboratorio comprende:

- Nodo soufe1: nodo front-end con HaProxy come reverse proxy.
- Nodo soube2: nodo back-end con Prometheus e Grafana gestiti tramite Podman.
- Tutte le configurazioni sono automatizzate tramite un Ansible role 'sou_podman'
- HaProxy instrada le richieste HTTP verso Prometheus e Grafana.

#Requisiti

- Vagrant
- VirtualBox o altro provider compatibile
- Ansible

#Come avviare il laboratorio

1. Clona il repository & avvio:
git clone https://github.com/samueleaudace-sourcesense/sou-lab-cni.git
cd sou-lab-cni
vagrant up

2. Accesso ai serivizi 
- HaProxy: 192.168.50.10:8080 / 8443  
- Prometheus: 192.168.50.10:9090  
- Grafana: 192.168.50.10:3000

