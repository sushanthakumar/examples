# SODA Kahu Project Integration with NTT

**Project :** Kahu - The SODA container data backup and restore project([https://github.com/soda-cdm/kahu](https://github.com/soda-cdm/kahu))

**User :** NTT MEC

**Use case :** To experience the container workload backup/restore for applications using kahu

**Description :**
- There are two environments: Docomo MEC's Kubernetes environment and the bare metal environment.
- Lab setup have kubernetes cluster setup on bare metal along with several deployed applications
- Netapp Trident storage is attached to the cluster
- SODA Kahu deployed on this cluster in a dedicated namespace
- Sample application is deployed on cluster which has storage and configuration requirements

- Below key scenarios are under test on the setup
    - Backup of entire namespace of the sample application
    - Backup of selected set of resources of the application
    - Restoration of the application from a specified backup
    - Execution of pre hook and post hook during backup and restore
- Testing on MEC has not been conducted yet and will be carried out in the future
- In the MEC, since we cannot directly access the storage appliance, there is a need to set up an NFS server
