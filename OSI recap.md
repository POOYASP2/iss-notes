# OSI recap

## Here are some networking recaps. I’m trying to cover everything I need for ISS.

No we have devices for networking.

### Devices

1.  Repeater: amplifies the signal (regenerates).
2.  Hub: multi-port repeaters (broadcasting).
3.  Bridge: sit between hub-connected hosts.
    1.  Only has two ports.
    2.  learns which hosts are on each side.
4.  Switches: combination of hubs and bridges. facilitate communication **within** a network.
    1.  multi ports.
    2.  learns which hosts are on each port. (How?? with creating a **hierarchy** in networks and the entire internet)
5.  Router: facilitate communication **between** networks.
    1.  provide traffic control point (security, filtering, redirecting)
    2.  routers have **routing tables** which are used for all the networks a router knows about.

![alt text](image.png)
_hierarchy of routers_

> **Note:** we have two terms, **switching** and **routing**. switching means moving data within a network and routing means moving data between networks. why I mention this? because other devices use this method too it is not mandatory we have just router and switches (even virtual ones).

### OSI model

Two host share data over. must hosts follow some rules.
Each layer provide and has specific purpose.

### Layer 1 (physical layer) - transporting bits

Fiber and wifi for example. repeater is a layer one device.

### Layer 2 Data link - Hop to Hop delivery

#### devices:

- **NICs** (like network interface cards or WIFI access card)
- **Switches**

Puts bits on the wire and receives bits from the wire. Anything which connected to the wire be the layer 2 devices (NIC - network interface cards, wifi access card)

The layer 2 uses MAC address for Hop top Hop delivery.

![alt text](hop-to-hop.png)
_Hop to Hop delivery_
