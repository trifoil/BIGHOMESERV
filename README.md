# BIGHOMESERV

## Table of Contents
1. [Installation of TrueNAS Scale](#installation)
2. [Disk Management and RAID Configuration](#disk-management)
   1. [Disk Management](#disk-management)
   2. [RAID Configuration](#raid-configuration)
3. [Setting up a VPN with a Domain Name](#vpn-setup)
   1. [Domain Name Registration (e.g., using Infomaniak)](#domain-registration)
   2. [VPN Configuration](#vpn-configuration)
4. [DNS Configuration](#dns-configuration)
5. [User Management](#user-management)
6. [Installation and Setup of GitLab](#gitlab-setup)
7. [Conclusion](#conclusion)

## Installation of TrueNAS Scale<a name="installation"></a>

This tutorial describes the web interface configuration

## Disk Management and RAID Configuration<a name="disk-management"></a>

This section covers the process of managing disks and setting up RAID configurations for TrueNAS Scale. This is crucial for ensuring data redundancy, performance, and storage capacity.

### Disk Management<a name="disk-management"></a>



### RAID Configuration<a name="raid-configuration"></a>

## Setting up a VPN with a Domain Name<a name="vpn-setup"></a>

### Domain Name Registration (e.g., using Infomaniak)<a name="domain-registration"></a>

### VPN Configuration<a name="vpn-configuration"></a>

## DNS Configuration<a name="dns-configuration"></a>

## User Management<a name="user-management"></a>

## Installation and Setup of GitLab<a name="gitlab-setup"></a>

## Conclusion<a name="conclusion"></a>

























RAID 0 (Striping):
RAID 0 combines two or more HDDs into a single volume, distributing data across them. It offers improved performance but provides no data redundancy or fault tolerance. If one drive fails, all data is lost.

RAID 1 (Mirroring):
RAID 1 involves duplicating data across two or more HDDs. It provides data redundancy and fault tolerance; if one drive fails, the others still have the data. However, it's less efficient in terms of storage capacity.

RAID 5 (Striping with Parity):
RAID 5 stripes data across multiple HDDs and also includes parity information for fault tolerance. It offers both performance and redundancy. If one drive fails, data can be reconstructed from the parity information.

RAID 10 (Combination of RAID 1 and RAID 0):
RAID 10 combines elements of both RAID 1 and RAID 0. It mirrors data (like RAID 1) and then stripes it for improved performance (like RAID 0). It offers both redundancy and performance, but it requires a minimum of four HDDs. If one drive fails in each mirrored pair, data is still accessible.

RAID 6 (Striping with Double Parity):
RAID 6 is similar to RAID 5 but includes double parity, which provides additional fault tolerance. It can withstand the failure of two HDDs simultaneously, making it more resilient than RAID 5.

RAID 50 (Combination of RAID 5 and RAID 0):
RAID 50 combines the striping of RAID 0 with the distributed parity of RAID 5. It provides both performance and redundancy, but it requires a minimum of six HDDs.

RAID 60 (Combination of RAID 6 and RAID 0):
RAID 60 combines the striping of RAID 0 with the dual parity of RAID 6. It offers high performance and robust fault tolerance, suitable for large storage arrays.

RAID 4 (Block-Level Striping with Dedicated Parity):
RAID 4 stripes data at the block level and uses a dedicated parity drive. It provides redundancy, but the dedicated parity drive can become a bottleneck in some cases.

RAID 3 (Byte-Level Striping with Dedicated Parity):
RAID 3 is similar to RAID 4 but stripes data at the byte level. It also uses a dedicated parity drive, which can limit performance in certain scenarios.

JBOD (Just a Bunch Of Disks):
JBOD doesn't provide RAID features but simply combines multiple HDDs into a single logical volume. Each drive is used sequentially, so there's no redundancy or performance improvement.