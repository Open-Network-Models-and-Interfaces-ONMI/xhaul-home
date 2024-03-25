# x-haul
Landing page of the x-haul working group in the ONMI project

The x-haul working group defines technology-specific extensions to the ONF Core Information Model (ONF TR-512).  
The individual modules can be flexibly combined and applied to different types of devices.  
The main focus of the working group is to make features and functions of state-of-the-art microwave devices available for vendor-independent configuration.  

The following types of extensions are distinguished:
- Interfaces are attached to the LayerProtocol class of the ONF Core IM and are used to manage network layers at the interfaces of devices.
- Profiles are attached to the new Profile class of the ONF Core IM and are used to manage functionality shared by multiple interfaces of a device.
- Connections are attached to the ForwardingDomain, Link or ForwardingConstruct class of the ONF Core IM and are used to document topology information of the respective network layer.

## Network Layers

### Air
* [airInterface](https://github.com/openBackhaul/airInterface) : Physical layer of the microwave radio interface

### EthernetContainer
- [ethernetContainer](https://github.com/openBackhaul/ethernetContainer) : Interface for sending and receiving frames
- [ethernetContainerFd](https://github.com/openBackhaul/ethernetContainerFd) : Potential of layer 1 forwarding of frames
- [ethernetContainerFc](https://github.com/openBackhaul/ethernetContainerFc) : Actual layer 1 forwarding of frames

### HybridMwStructure
* [hybridMwStructure](https://github.com/openBackhaul/hybridMwStructure) : Structuring of a microwave radio interface into multiple TDM and a single Ethernet segment

### IP
- [ipInterface](https://github.com/openBackhaul/ipInterface) : IPv4 interface according to IETF RFC 791

### MAC
- [macInterface](https://github.com/openBackhaul/macInterface) : Ethernet MAC interface according to IEEE 802.1
- [macFd](https://github.com/openBackhaul/macFd) : Potential forwarding (MAC switch) according to IEEE 802.1
- [lldp](https://github.com/openBackhaul/lldp) : Link Layer Discovery Protocol according to IEEE 802.1AB

### PureEthernetStructure
- [pureEthernetStructure](https://github.com/openBackhaul/pureEthernetStructure) : Structuring of a microwave radio interface into a single Ethernet segment

### Synchronization
- [synchronization](https://github.com/openBackhaul/synchronization) : Synchronization model according to ITU-T G.7721-2018

### TdmContainer
- [tdmContainer](https://github.com/openBackhaul/tdmContainer) : Transport resource for TDM

### VLAN
- [vlanInterface](https://github.com/openBackhaul/vlanInterface) : VLAN interfaces (Port) according to IEEE 802.1Q
- [vlanFd](https://github.com/openBackhaul/vlanFd) : Potential forwarding (Component) according to IEEE 802.1Q
- [vlanFc](https://github.com/openBackhaul/vlanFc) : Actual forwarding (VLAN) according to IEEE 802.1Q

### Wire
- [wireInterface](https://github.com/openBackhaul/wireInterface) : Physical layer of an Ethernet PHY interface according to IEEE 802.3

## Profiles
- [coChannelProfile](https://github.com/openBackhaul/coChannelProfile) : Groups of microwave radio interfaces, which are using the same frequency channel
- [l3vpnProfile](https://github.com/openBackhaul/l3vpnProfile) : Layer 3 Virtual Private Networks
- [policingProfile](https://github.com/openBackhaul/policingProfile) : Regulation of the flow by rates and burst sizes
- [qosProfile](https://github.com/openBackhaul/qosProfile) : Quality of Service based on 802.1p, MPLS Exp and IP DSCP
- [schedulerProfile](https://github.com/openBackhaul/schedulerProfile) : Scheduler for sending frames
- [wredProfile](https://github.com/openBackhaul/wredProfile) : WRED (Weighted Random Early Detection)

## Core
- [backupAndRestore](https://github.com/openBackhaul/backupAndRestore) : Information model and RPCs for managing backup and restore on the device
- [core](https://github.com/openBackhaul/core) : Core Information Model that consolidates all Interfaces, Profiles and Equipments
- [ltpAugment](https://github.com/openBackhaul/ltpAugment) : Technology agnostic amendment to the LogicalTerminationPoint class
- [firmware](https://github.com/openBackhaul/firmware) : Information model and RPCs for managing firmware on the device
- [equipment](https://github.com/openBackhaul/equipment) : Device Inventory, Device type specific Information and Interface Behavior
- [alarms](https://github.com/openBackhaul/alarms) : Centralized representation of alarms
- [notifications](https://github.com/openBackhaul/notifications): Generic notifications
