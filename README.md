# Printer Monitoring Stack for Klipper Printers

This is a simple docker-compose setup for a server and a second part for printers running klipper to be able to monitor them and have a better insight into what is happening during print failures.

## Server Setup

### Install Docker
[Install Docker](https://docs.docker.com/engine/install/)

### Pull config from repo

```sh
git clone repo
```

### Ensure secrets files are populated with required info

Make sure to update the info in ./secrets/

### Check over the .env file for any changes needed.

```sh
vi .env
```

Scroll through and check for any field that needs to be updated for your particular environment.

## Starting the server

```
docker compose up -d
```

## Updating the server

```
docker compose pull
docker compose up -d
```

# Accessing Grafana
