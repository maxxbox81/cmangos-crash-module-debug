# cmangos-crash-module-debug

Patch collection to fix crashes and stability issues in CMaNGOS modules (e.g., PlayerBots, TrainingDummies, etc.)
➡️ Core-related crash patches are available at [cmangos-crash-debug](https://github.com/maxxbox81/cmangos-crash-debug)

## 🛠️ Included Patches

| Patch File | Description | Crash Screenshot |
|------------|-------------|------------------|
| [M0001-fix-NamedObjectContext-nullptr-crash.patch](M0001-fix-NamedObjectContext-nullptr-crash.patch) (Playerbots) | Fixes a potential crash when NamedObjectContext::create() returns a null pointer | [1️⃣ View](images/M0001_1_Namedobjectcontect.png)<br>[2️⃣ View](images/M0001_2_Namedobjectcontect.png) |
| [M0002-fix-EmptyChatcrash.patch](M0002-fix-EmptyChatcrash.patch) (Playerbots) | Prevent crash in PlayerbotAI by validating strings and null pointers in queued chat replies | [1️⃣ View](images/M0002-fix-EmptyChatcrash.png)<br> |
| [M0003-fix-last-said-nullptr.patch](M0003-fix-last-said-nullptr.patch) (Playerbots) | Prevent crash in PlayerbotAI empty nullptr "last said" "chat" | [1️⃣ View](images/M0003-fix-last-said-nullptr.png)<br> |
| [M0004-fix-dualspecc-menu.patch](M0004-fix-dualspecc-menu.patch) (Dualspec) | Fix dualspec gossip menu | [1️⃣ View](images/M0004-fix-dualspecc-menu.png)<br> |

## 💡 Usage

```bash
cd /opt/cmangos/mangos
git apply /opt/cmangos/mangos/patches/modules/M0001-fix-NamedObjectContext-nullptr-crash.patch
git apply /opt/cmangos/mangos/patches/modules/M0002-fix-EmptyChatcrash.patch

