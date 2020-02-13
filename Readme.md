# Wordpress on Cloud
    
A quick guide about how to setup a Wordpress installation with your own theme and plugins on a managed Kubernetes and a managed MySQL cluster.

**_NOTE_: Wordpress files included in this repo are only for demo purposes. Once the installation is completed make sure to update. Click [http://wordpress.org/download](here) to access the leates WP release.**

## Prerequisites

- [https://kubernetes.io/docs/tasks/tools/install-kubectl/](kubectl)
- [https://docs.docker.com/install/](Docker)
- You will also need a Docker [https://hub.docker.com/](Hub) account to host the customized image we will create.
- Account to the cloud provider you wish to use.

**_NOTE_: Please check the pricing policy of the cloud provider you will use as costs might apply regarding the deployment of each of the solution in this repo.**

## Explanation of folders

We have put each solution for the cloud provider we support in a seperate folder with the related name. Each folder has the following structure:

- doc: A detailed guide for the steps to have our WP installation up and running.
- wordpress: The WP files (including our theme & plugins that will be used for the installation).
- YAML files to setup the Kubernetes cluster.
- Dockerfile to build the required image.

## Accountability Notice

Instructions and files provided in this repository should be used as is and are provided only for educational purpose and not for professional purposes. Costs may apply in case you deploy to a cloud provider.