---
description: Configuring the tools required to begin ONT ID integration
---

# Environment and tools

This section lays out the tools needed to work with the ONT ID framework and carry out the integration process. 

### Docker

Docker is a OS-level virtualization engine used for software development and testing.We will use a Docker image provided by Ontology to serve as the **signing server**.

Docker can be downloaded by following the link below. It is necessary to sign up for Docker before downloading it.

[https://www.docker.com/get-started](https://www.docker.com/get-started)

This signing server developed by Ontology serves to set up a decentralized identity application server that can be used to deploy individual web apps.

Once docker is installed and running, run the following command to mount the image.

```bash
docker run -p 8099:8099 -v /host_mnt/d/docker/signing-server/config/:/config -v /host_mnt/d/docker/signing-server/logs/:/logs --name signing signing-server_signing-server
```

{% hint style="warning" %}
 The _application.properties_ configuration file also needs to be mounted.
{% endhint %}

### ONT Auth

**ONT Auth** is a personal claim management application developed by Ontology that facilitates self sovereign identity management using `ONT ID`.

The application is available for both Android and iOS systems, can can be downloaded by following the link below. 

_**\*\*Add link\*\***_

_\*\*\*\*_



