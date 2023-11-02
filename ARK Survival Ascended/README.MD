# 🦖 ARK: Ascended Server Setup 🚀

This guide will take you on a journey to set up the ARK: Ascended game server! Let's dive right in.

## 📝 Prerequisites
- Ensure you're wearing your adventurer's hat! 🎩 (Just kidding, but do ensure you have `sudo` privileges.)

## 🛠 Instructions

### 1️⃣ Directory Setup
Whip up the required directory with:
```bash
mkdir /home/customer/service-data/arksa
cd /home/customer/service-data/arksa
```

### 2️⃣ Install DepotDownloader
Get the tools you need:
```bash
sudo yum install DepotDownloader -y
```

### 3️⃣ Download the ARK Files
🔍 Need the latest manifest ID? Find it [here](https://steamdb.info/app/2430930/depots/?branch=public).

Now, summon the files:
```bash
/usr/local/bin/DepotDownloader -app 2430930 -depot 2430931 -manifest 4326933906237823815 -dir .
```

### 4️⃣ Power Up!
Give the server executable the power it deserves:
```bash
chmod +x ShooterGame/Binaries/Win64/ArkAscendedServer.exe
```

## 🎉 Conclusion
Your ARK: Ascended server is now set up and roaring to go! 🦕 Regularly check the SteamDB link above for any updates to ensure your server remains in its prime!

Happy gaming! 🎮