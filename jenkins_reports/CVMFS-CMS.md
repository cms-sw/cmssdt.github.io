# [CVMFS-CMS](https://cmssdt.cern.ch/jenkins/view/CVMFS-CMS)

**View description:** None

**View type:** List View

---

# Projects:

## [cvmfs-cms-eos-list](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-eos-list)

**Description:** None

**Project is `enabled`.**

**Upstream projects:**
* [cvmfs-cms-eos-sync](#cvmfs-cms-eos-sync):

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-eos-sync](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-eos-sync)

**Description:** None

**Project is `enabled`.**

**Upstream projects:**

**Downstream projects:**
* [cvmfs-cms-eos-list](#cvmfs-cms-eos-list):

**Sub-projects:**
* [cvmfs-cms-eos-list ](#cvmfs-cms-eos-list ):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-eos-sync-dirs](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-eos-sync-dirs)

**Description:** Sync two folders with  cvmfs transaction.
If the destination folder is on cvmfs, it gets published 

**Project is `enabled`.**

**Upstream projects:**
* [cvmfs-cms-update-gridpacks](#cvmfs-cms-update-gridpacks):

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-cms](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-cms)

**Description:** Job to install (test) releases (and IBs) once the upload is completed.
The job should be triggered by upstream job upload-release.
It's purpose is to only trigger cms-install-package with the same argument
it would get from upload-release job, but without using upload-release instance (it's just a trigger job for now)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-common](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-common)

**Description:** Trigger the installation of new production architecture for CMS or reinstall cms-common new revision.<br/>
- Production architecture if obtained via <a href="https://raw.githubusercontent.com/cms-sw/cms-bot/master/config.map">config.map</a><br/>
This job is triggered by <a href="https://cmssdt.cern.ch/jenkins/job/cmsrep-webhook">cmsrep-webhook</a> which should pass the cms-common revision and architecture.

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-COMP-python](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-COMP-python)

**Description:** Job to install python whenever there is a new version pushed on cmsrep.cern.ch <br>
Install path is ${CVMFS_PATH} + COMP install dir (boostraped for comp)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-COMP-xrootd](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-COMP-xrootd)

**Description:** Job to install xrootd whenever there is a new version pushed on cmsrep.cern.ch <br>
Install path is ${CVMFS_PATH} + COMP install dir (boostraped for comp)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-crab3](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-crab3)

**Description:** Job to install crab3 whenever there is a new version pushed on cmsrep.cern.ch <br>
Install path is ${CVMFS_PATH} + crab3 install dir (boostraped for comp)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-package](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-package)

**Description:** This job installs packages using cmspkg tool
To be used for - CRAB3, PHEDEX, spacemon-client, python, releases(cmssw), cms-common
Triggered by webhook

**Project is `enabled`.**

**Upstream projects:**
* [cvmfs-cms-install-COMP-python](#cvmfs-cms-install-COMP-python):
* [cvmfs-cms-install-COMP-xrootd](#cvmfs-cms-install-COMP-xrootd):
* [cvmfs-cms-install-cms](#cvmfs-cms-install-cms):
* [cvmfs-cms-install-common](#cvmfs-cms-install-common):
* [cvmfs-cms-install-crab3](#cvmfs-cms-install-crab3):
* [cvmfs-cms-install-phedex](#cvmfs-cms-install-phedex):
* [cvmfs-cms-install-spacemon-client](#cvmfs-cms-install-spacemon-client):

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-phedex](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-phedex)

**Description:** Job to install phedex whenever there is a new version pushed on cmsrep.cern.ch <br>
Install path is ${CVMFS_PATH} + phedex install dir (boostraped for comp)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-install-spacemon-client](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-install-spacemon-client)

**Description:** Job to install spacemonclient whenever there is a new version pushed on cmsrep.cern.ch <br>
Install path is ${CVMFS_PATH} + spacemonclient install dir (boostraped for comp)

**Project is `enabled`.**

**Upstream projects:**
* [cmsrep-webhook](#cmsrep-webhook):

**Downstream projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Sub-projects:**
* [cvmfs-cms-install-package](#cvmfs-cms-install-package):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-update-git-mirror](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-update-git-mirror)

**Description:** This job mirrors cmssw to cms.cern.ch as described here:

https://github.com/bockjoo/cvmfs-cms-install-scripts/blob/master/update_cmssw_git_mirror.sh#L191
Thats the only function that executes, as it exits right after:
https://github.com/bockjoo/cvmfs-cms-install-scripts/blob/master/update_cmssw_git_mirror.sh#L50


**Project is `enabled`.**

**Upstream projects:**

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-update-gridpacks](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-update-gridpacks)

**Description:** This job updates gridpacks on cvmfs as described here:
<br> https://github.com/mrodozov/cvmfs-cms-install-scripts/blob/master/cron_rsync_generator_package_from_eos_individual.sh

**Project is `enabled`.**

**Upstream projects:**

**Downstream projects:**
* [cvmfs-cms-eos-sync-dirs](#cvmfs-cms-eos-sync-dirs):

**Sub-projects:**
* [cvmfs-cms-eos-sync-dirs](#cvmfs-cms-eos-sync-dirs):

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-update-lhapdf](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-update-lhapdf)

**Description:** This job updates gridpacks on cvmfs as described here:
<br> https://github.com/mrodozov/cvmfs-cms-install-scripts/blob/master/cron_rsync_generator_package_from_eos_individual.sh

**Project is `enabled`.**

**Upstream projects:**

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---

## [cvmfs-cms-update-siteconf](https://cmssdt.cern.ch/jenkins/job/cvmfs-cms-update-siteconf)

**Description:** This job updates SITECONF on cvmfs as described here:
<br> https://github.com/mrodozov/cvmfs-cms-install-scripts/blob/master/cron_install_cmssw.sh#L562 

**Project is `enabled`.**

**Upstream projects:**

**Downstream projects:**

**Sub-projects:**

**Triggers from:** []


**Periodic builds:**
```bash
Not periodically build
```

---
