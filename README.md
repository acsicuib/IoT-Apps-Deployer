This is the tool developed for lighweight deployment of IoT applications and presented in the article "A Platform for Lightweight Deployment of IoT Applications Based on a Function-as-a-Service Model", accepted for publication in IEEE Latin America Transactions. For more details, please, read the article in https://doi.org/10.1109/TLA.2019.8931204

Serveral modules have been developed: the central server, the fog node module, the monitoring scripts and the raspbian images as example of fog node. 

**Please consider to cite this work as**:

```bash
@ARTICLE{8931204,
  author={Sanso, Sebastia and Guerrero, Carlos and Lera, Isaac and Juiz, Carlos},
  journal={IEEE Latin America Transactions}, 
  title={A Platform for Lightweight Deployment of IoT Applications Based on a Function-as-a-Service Model}, 
  year={2019},
  volume={17},
  number={07},
  pages={1155-1162},
  doi={10.1109/TLA.2019.8931204}}
```

**Acknowledgment**:

This research was supported by the Spanish Government (Agencia Estatal de Investigación) and the European Commission (Fondo Europeo de Desarrollo Regional) through Grant Number TIN2017-88547-P (AEI/FEDER, UE).


# Servidor central

Steps:

- Imagen
  - Rasbian Jessie
  
- Node
  - curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
  - sudo apt-get install -y nodejs

- Mongo
  - sudo apt-get update
  - sudo apt-get upgrade
  - sudo apt-get install mongodb-server
  - sudo service mongodb start

# Monitoring Scripts
Scripts en Python para monitorizar con las raspberry.

# Nodo

- sudo nano /etc/rc.local
  - nohup python /home/pi/Node/nodo/scripts/init.py &

# raspbian_link

Raspbian image url: https://mega.nz/#!y0IQDZZB!g8zi5njLHpqipZ9p8cGZVegP2uhGHcfq232h7SLjRCU
