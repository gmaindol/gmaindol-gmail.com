# HA Clustering

Palo Alto Networks firewall models (Hardware Firewall and VMseries) now support session state synchronization among firewalls
in a high availability (HA) cluster of up to 16 firewalls. The HA cluster peers synchronize sessions to protect against failure of link or device. If a link or device goes down, the sessions fail over to a different firewall in the cluster.


# HA Cluster Configuration
HA Cluster configuration skillet provides quick an easy way to configure an HA cluster across devices. With this skillet customer can configure HA cluster on multiple devices and assign them to their respective HA clusters.

With this skillet following setting are configured on the device

Configure HA ethernet interface
Enable HA cluster with unique cluster id
Set cluster members config
Configure HA4 and HA4-backup interface

# Prerequisite
1) HA cluster members must be of same firewall model and run the same PAN-OS® version
2) Connect HA communication interfaces and make sure link state is up
3) Peer member’s Device Serial Number
4) Panorama is highly recommended to ensure that HA cluster memeber have consistent policies

# Support Policy
The code and templates in the repo are released under an as-is, best effort, support policy. These scripts should be seen as community supported and Palo Alto Networks will contribute our expertise as and when possible. We do not provide technical support or help in using or troubleshooting the components of the project through our normal support options such as Palo Alto Networks support teams, or ASC (Authorized Support Centers) partners and backline support options. The underlying product used (the VM-Series firewall) by the scripts or templates are still supported, but the support is only for the product functionality and not for help in deploying or using the template or script itself. Unless explicitly tagged, all projects or work posted in our GitHub repository (at https://github.com/PaloAltoNetworks) or sites other than our official Downloads page on https://support.paloaltonetworks.com are provided under the best effort policy.
