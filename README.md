capbash-cadvisor
==============

Scripts for deploying [cadvisor](https://github.com/google/cadvisor) for monitoring docker containers

# How to Install #

Install capbash first, more details at:
https://github.com/aforward/capbash

```
curl -s https://raw.githubusercontent.com/aforward/capbash/master/capbash-installer | bash
capbash new YOUR_REPO_ROOT
cd YOUR_REPO_ROOT
```

Now you can install cadvisor into your project

```
capbash install cadvisor
```

# Configurations #

The available configurations include:

```
CADVISOR_LAUNCHER_DIR=${CADVISOR_LAUNCHER_DIR-/var/local/cadvisor}
CADVISOR_PORT=${CADVISOR_PORT-8080}
```

# Deploy to Remote Server #

To push the cadvisor script to your server, all you need if the IP or hostname of your server (e.g. 192.167.0.48) and your root password.

```
capbash deploy <IP> cadvisor
```

For example,

```
capbash deploy 127.0.0.1 cadvisor
```
