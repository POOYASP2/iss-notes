# Firewall

**Q -** What is a Firewall ?

> A firewall is a security system that enforce controlled communication between networks of different security levels. It acts as a boundary protection point, filtering traffic according to defined authorization policies to prevent unauthorized access between trusted and untrusted domains.

**Q -** What is a ingress firewall ?

> An ingress firewall is a firewall configuration that inspects and controls the incoming network traffic from an untrusted network toward a trusted network. Its purpose is typically to select which service from inner network (trusted network) is opened for untrusted or outer network.

**Q -** What issue may we face with an ingress firewall?

> In some cases, an internal program inside the trusted network may want to open and make a connection with the outside network.

**Q -** What is an egress firewall?

> An egress firewall is a firewall configuration that inspects and controls outgoing network traffic from the trusted network toward an untrusted network (from the inner to the outer network). The purpose of this configuration is to control user actions within a network, such as determining which sites a user can access, preventing users from uploading sensitive information to the external network, or blocking the download of potentially dangerous files.

**Q -** Why we can not always have clear distinguish between ingress and egress?

> Because classification between egress and ingress is straightforward for **channel-based** services such as TCP applications, but for **message-based** services such as UDP applications we do not have this clear distinction, and the firewall in this case is typically bidirectional.

**Q -** What is the primary consideration in designing a firewall?

> The primary consideration is the desired security level.

Note: The higher the protection level, the fewer functionalities can be provided.

**Q -** What are the commandments of the firewall?

> 1. The firewall must be only contact point of the internal network with the external one.
> 2. Only the "authorized" traffic can traves the firewall.
> 3. The firewall must be a highly secure system itself.

**Q -** Why must the firewall be the only contact point between the internal network and the external network?

> Because when we use a firewall, we want to have centralized control over all communications. If any nodes can access the external network through a different contact point rather than the firewall, we cannot have centralized control, and we will have some unmonitored and unfiltered communications which can create vulnerabilities for our trusted network.

**Q -** Why must only authorized traffic traverse the firewall?

> Because allowing only authorized traffic through the firewall ensures that every connection entering or leaving the trusted network is **inspected**, **controlled**, and **compliant** with the organization’s security policies.  
> Unauthorized traffic could bypass these controls and introduce malware, attacks, data leaks, or unknown communication channels, which would compromise the security and integrity of the internal network.

**Q -** What are the types of authorization policies in the firewall?

> 1. Whitelisting: All that is not explicitly permitted is forbidden.
> 2. BlackListing: All that is not explicitly forbidden is permitted.

**Q -** What are the characteristics of a whitelisting policy in firewalls?
