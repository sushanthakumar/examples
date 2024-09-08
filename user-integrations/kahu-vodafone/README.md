# SODA Kahu Project Integration with Vodafone

**Project :** Kahu - The SODA container data backup and restore project([https://github.com/soda-cdm/kahu](https://github.com/soda-cdm/kahu))

**User :** Vodafone

**Use case :** To experience the container workload backup/restore for applications using kahu

**Description :**
- Lab setup have RHOCP cluster along with several deployed application
- Kahu Version : v1.1.0
- Test were executed with storage emulation and with Dell PowerStore storage providing volumes to the RHOCP cluster
- SODA Kahu deployed on this cluster in a dedicated namespace
- Sample application is deployed on cluster which has storage and configuration requirements

- Below key scenarios are verified on the setup
    - Backup of entire namespace of the sample application
    - Backup of selected set of resources of the application (pod, configmap, service, persistent volume, persistent volume claim, storage class )
    - Restoration of the application from a specified backup
    - Execution of pre hook and post hook during backup and restore

**Next Step :**
- Currently Kahu supports volume backup through storage side snapshots. Feature to support backup to remote repositories is still in progress - Dev in progress. 
- Vodafone likes to test this feature as soon as is available
- To experience the RHOCP infrastructure backup/restore (RHOCP component level)
