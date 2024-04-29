# Welcome to openEBS
[![OpenEBS Social Banner](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_main_banner_HERO_1.png)](https://www.openebs.io/)

## [openebs.io](https://www.openebs.io/)
OpenEBS is a opensource Stateful Persistent block-mode Data Storage platform for Kubernetes. We are CNCF member project. We are a large global community of K8s Data storage users.<BR>
<BR>
Our project team was an early pioneering inventor of K8s **Container Native Storage** services. We concieved the vision of a Stateful Persistent data platform for K8s that is tightly integrated and natively embeded into the core of K8s.<BR>
<BR>
We have built an innovative ultra High-performance Enterprise grade Block-mode Hyper-converged Data Storage Fabric that augments the core storage services of K8s with Stateful Persistence, Enterprise Data mgmt, SSD/NVMe optimized I/O services, Replicated Data volumes, Thin Provisioning, Snapshot and Clones; and many other critical data storage services that don't come in K8s out-of-the-box.<BR>
<BR>

> **OpenEBS is very popular** : Live OpenEBS systems actively report back product metrics every day, to our Global Anaytics metrics engine (unless disabled by the user).
> Here are our key project popularity metrics as of: 01 Feb 2024 <BR>
>
> :rocket: &nbsp; OpenEBS is the #1 deployed Storage Platform for Kubernetes <BR>
> :star: &nbsp; We are the [#1 GitHub Star ranked](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png) K8s Data Storage platform <BR>
> :floppy_disk: &nbsp; We have +49 Million Volumes deployed globally <BR>
> :tv: &nbsp; We have +8 Million Global installations <BR>
> :zap: &nbsp; 1 Million OpenEBS K8s Containers are spawned per week <BR>
> :sunglasses: &nbsp; 1.1 Million global users <BR>

| [![coders](https://github.com/openebs/website/blob/main/website/public/images/png/code_icon_200x100.png "Write more awesome code")](https://github.com/openebs/website/blob/main/website/public/images/png/website/public/images/png/code_for_success_mantra_small.png)  | Building a K8s Enterprise Data Storage platform is complex, and areas of the Data & I/O stack could be considerd 'Storage Rocket science'. Our global team comes from many areas of the data storage industry. Companies like... [Microsoft Azure](https://azure.microsoft.com/en-us/), [VMware](https://www.vmware.com/), [DELL/EMC](https://www.dell.com/en-us/shop/scc/sc/storage-products), [Brocade/Broadcom](https://www.broadcom.com/products/fibre-channel-networking), [Hitachi Vantara](https://www.hitachivantara.com/en-us/products/storage-platforms.html), [INTEL](https://www.intel.com/content/www/us/en/products/details/memory-storage.html), [Nvidia/Mellanox](https://developer.nvidia.com/gpudirect-storage), [IBM](https://www.ibm.com/storage), [RedHat](https://www.redhat.com/en/technologies/cloud-computing/openshift) and [DataCore](https://datacore.com).  |
| :---  | :--- |
<BR>

> [!IMPORTANT]
> We are grateful for the above innovative Data Storage companies and their amazing engineering contributors. Our orignal founding team continues to guide the project as custodial Maintainers. Major sponsorship is provided by [DataCore](https://datacore.com), who donates a large team of dedicated  Product Dev/Engineers, Product Mgmt and operational rescources. (Our founding team was acquired by DataCore, Inc). OpenEBS has 100's of amazing individuals, contributors and storage engineers who provide brainstorming ideas, feedback, code reviews and high-quality code to the project. - All who are passionate about storage and Data are welcome here.

## Project structure
[![Project Structure](https://github.com/openebs/website/blob/main/website/public/images/png/openebs_github_project-structure_april2024.png)](https://github.com/openebs/community/)

## Deployable Data-Engines
OpenEBS has maintained a steady pace of development & evolution in order to keep in alignment with K8s advancment overall and with the rapid changing pace of technologies, hardware and software innovations in the data stroage industry. The proejct is divided into 2 main deployable Editions :<BR>
| ID  | Edition name  | Data-Engine | Release        |
|-----|---------------|-------------|----------------|
|  1  | ```Legacy```        | [cStor](https://github.com/openebs/cstor-operators)       | [![Releases](https://img.shields.io/github/v/release/openebs/cstor-csi.svg?include_prereleases&style=flat-square)](https://github.com/openebs/cstor-csi/releases)   |
|     |               | [Jiva](https://github.com/openebs/jiva)  | [![Releases](https://img.shields.io/github/v/release/openebs/jiva.svg?include_prereleases&style=flat-square)](https://github.com/openebs/jiva/releases)   |
|     |               | [NFS](https://github.com/openebs/dynamic-nfs-provisioner)  |    |
|  2  | ```Standard```     | [Mayastor](https://github.com/openebs/mayastor)     | [![Releases](https://img.shields.io/github/release/openebs/Mayastor/all.svg?style=flat-square)](https://github.com/openebs/Mayastor/releases)   |
<BR>

## ```LEGACY Edition```
> [!NOTE]
> ```
> LEGACY consists of Data-Engines that we experimented with early on. These Data-Engines have a number of opensoruce
> techologies embeded inside them, and are a great intro into the world of simple K8s storage services. LEGACY helped
> us learn, iterate and develop our core storage K8s strategy, as well as decern how users want & need to interact with
> K8s storage services. LEGACY also helped to reveal key areas within K8s that are lacking in storage/datastore services,
> what areas of K8s we could optimize; and how we can provide the best value into the various K8s storage layers.

There are multiple Data-Engines within LEGACY:<BR>
| ID  | Data-Eegines      | Embeded tech stack   | Status                           |
|-----|-------------------|----------------------|----------------------------------|
|  1  |  Jiva             | iSCSI                | Has been ```deprecated```. Will be migrating out of org soon  |
|  2  |  cStor            | Open ZFS             | Has been ```deprecated```. Will be migrating out of org soon |
|  3  |  NFS Provisioner  | NFS userspace server | Has been ```deprecated```. Will be migrating out of org soon |
|  4  |  Device LocalPV     | Node Local storage   | Has been ```deprecated```. Will be migrating out of org soon |
|  5  |  LocalPV Device     | Node Local storage   | Has been ```deprecated```. Will be migrating out of org soon |
|  6  |  NDM              | Node Local storage   | Has been ```deprecated```. Will be migrating out of org soon |
|  7  |  Many other tools   | Node Local storage   | Has been ```deprecated```. Will be migrating out of org soon |
<BR>


## ```STANDARD Edition```
**STANDARD** is our Ultra modern Datastore stack that is strongly aligned with the cutting edge direction of storage use-cases in the K8s industry. It is designed to faciliate modern K8s datastore archiectures, key K8s I/O patterns, K8s data access methods, K8s data use-cases and where K8s Datastore applications are heading.
<BR>	

 
STANDARD is optimized for NVMe and SSD Flash storage media, and integrates ultra modern cutting-edge high performance storage technologies at its core...</summary>

>
> :ballot_box_with_check: &nbsp; It uses the High performance [SPDK](https://spdk.io) storage stack - (SPDK is an opensource NVMe project initiated by INTEL) <BR>
> :ballot_box_with_check: &nbsp; The hyper modern [IO_Uring](https://github.com/axboe/liburing) Linux Kernel Async polling-mode I/O Interface - (fastest kernel I/O mode possible) <BR>
> :ballot_box_with_check: &nbsp; Native abilties for RDMA and Zero-Copy I/O <BR>
> :ballot_box_with_check: &nbsp; NVMe-oF TCP Block storage Hyper-converged data fabric <BR>
> :ballot_box_with_check: &nbsp; Block layer volume replication <BR>
> :ballot_box_with_check: &nbsp; Logical volumes and Diskpool based data managment <BR>
> :ballot_box_with_check: &nbsp; a Native high peformance [Blobstore](https://spdk.io/doc/blob.html) <BR>
> :ballot_box_with_check: &nbsp; Native Block layer Thin provisoning <BR>
> :ballot_box_with_check: &nbsp; Native Block layer Snapshots and Clones <BR>

</details>
<BR>


There are 2 Data-Engines within the [**STANDARD**](https://github.com/openebs/mayastor) Edition:
| ID  | Data-Eegines       | Type of data services                                  | Status                                                     |
|-----|--------------------|--------------------------------------------------------|------------------------------------------------------------|
|  1  |  ```Replicated``` <BR>[Mayastor](https://github.com/openebs/mayastor)      | Replicated data volumes (a Cluster wide Data fabric)   | Stable, deployable in PROD. Very active development        |
|     | &nbsp;             |                                                        |                                                            |
|  2  |  ```Local``` <BR>**LocalPV-xxx**       | Non-replicated node local data volumes                 | (Local-PV has multiple variants. See below)                |
|     |  [LocalPV-HostPath](https://github.com/openebs/dynamic-localpv-provisioner) | for integration with local node hostpath (e.g. /mnt/fs1)    | Stable, deployable in PROD, undergoing integration         |
|     |  [LocalPV-ZFS](https://github.com/openebs/zfs-localpv)      | for integration with local ZFS storage deployments          | Stable, deployable in PROD, undergoing integration         |
|     |  [LocalPV-LVM](https://github.com/openebs/lvm-localpv)      | for integration with local LVM2 storage deployments          | Stable, deployable in PROD, undergoing integration         |
|     |  [LocalPV-Raw-device-File](https://github.com/openebs/rawfile-localpv)    | for integration with Loop mounted Raw device-file filesystem | Stable, deployable in PROD, undergoing integration         |
<BR>

## :earth_americas: ROADMAP
Our [2024 Roadmap is here](https://github.com/openebs/openebs/blob/main/ROADMAP.md) It defines a rich set of new featrues that are planned for 2024.<br>
Please review this roadmp and feel free to pass back any feedback on it, as well as recommend and suggest new ideas. We welcome all your feedback.
<br>
<br>

## :star: GitHub Star Chart
OpenEBS is the most successful Stateful Persistent Contianer Native Storage platform in the CNCF landscape. It has allways held the #1 position and continues to as of today.

[![XXXXXXXX](https://github.com/openebs/website/blob/main/website/public/images/png/github_star-history-2024_Feb_1.png)](https://www.openebs.io/)
