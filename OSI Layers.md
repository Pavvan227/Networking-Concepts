# A deepdive into OSI model

**OSI - Open Systems interconnection**

TCP/IP model is the most commonly used, both models will provide the same responsibilities. Only sifference between them is how responsibilities are distributed among the layers.

![OSI Model](https://raw.githubusercontent.com/Pavvan227/Networking-Concepts/main/assets/OSI-7-layers.jpg)

## Layer 1: PHYSICAL Layer
This layer is reponsible for carrying raqbits on a physical medium. A physical medium could be physical wires or wireless connection between two nodes.
- Data unit: Bits
- Delivery type: Local

## Layer 2 : DATA LINK Layer
This layer is responsible for providein local delivery of frames between two directly connected devices. This layer has 2 componenets:

**1. Media Access Control(MAC)**
The MAC component controls the transmission and reception from the physical medium of layer 1. It employs either the Carrier Sense Multi Access with Collision Detection(CSMA/CD) or Carrier Sense Multi Access with Collision Avoidance(CSMA/CA) algorithm for this purpose.

Its main responsibilities include:
  - Check wheather the physica layer is free. If yes, trasmit, otherwise receive.
  - Check if any collision occured while transmitting. If yer, it sends a jam signal to instruct other hosts to stop transmitting, it then timeout for a random period of time and then attempts transmission.

**2. Logical link Control(LLC)**
