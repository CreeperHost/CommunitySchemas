# Dystopia Game Server Setup

This guide provides a step-by-step setup for the Dystopia game server. 

## Prerequisites

- Ensure you have `sudo` privileges on the server to perform installations.

## Instructions

### 1. Directory Setup

Create and navigate to the required directory:

```bash
mkdir /home/customer/service-data/dystopia
cd /home/customer/service-data/dystopia
```

### 2. Install DepotDownloader

Install the DepotDownloader package:

```bash
sudo yum install DepotDownloader -y
```

### 3. Download Required Files

Ensure that you have the correct manifest ID. You can check the latest manifest ID at [SteamDB - Dystopia](https://steamdb.info/app/17585/depots/).

Run the following commands to download the necessary game files:

```bash
/usr/local/bin/DepotDownloader -app 244310 -depot 244313 -manifest 6299109015578496445 -dir .
/usr/local/bin/DepotDownloader -app 17585 -depot 806641 -manifest 2070697226601717144 -dir .
/usr/local/bin/DepotDownloader -app 17585 -depot 17581 -manifest 7649529834308003280 -dir .
```

### 4. Assign Executable Permissions

Provide the necessary executable permissions:

```bash
chmod +x srcds_run
chmod +x bin/linux32/srcds
```

## Conclusion

Your Dystopia game server should now be set up. Regularly check the SteamDB link above for updates or changes to the manifest IDs to ensure your server remains updated.