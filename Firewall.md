# Firewall

**Q -** What is a Firewall ?

> A firewall is a security system that enforce controlled communication between networks of different security levels. It acts as a boundary protection point, filtering traffic according to defined authorization policies to prevent unauthorized access between trusted and untrusted domains.

**Q -** What is a ingress firewall ?

> An ingress firewall is a firewall configuration that inspects and controls the incoming network traffic from an untrusted network toward a trusted network. Its purpose is typically to select which service from inner network (trusted network) is opened for untrusted or outer network.

**Q -** What issue may we face with an ingress firewall?

> In some cases, an internal program inside the trusted network may want to open and make a connection with the outside network.

**Q -** What is an egress firewall?

> An egress firewall is a firewall configuration that inspects and controls outgoing network traffic from the trusted network toward an untrusted network (from the inner to the outer network). The purpose of this configuration is to control user actions within a network, such as determining which sites a user can access, preventing users from uploading sensitive information to the external network, or blocking the download of potentially dangerous files.
