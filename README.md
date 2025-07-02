# cmangos-crash-module-debug

Patch collection to fix crashes and stability issues in CMaNGOS modules (e.g., PlayerBots, TrainingDummies, etc.)
➡️ Core-related crash patches are available at [cmangos-crash-debug](https://github.com/maxxbox81/cmangos-crash-debug)

## 🛠️ Included Patches

| Patch File | Description | Crash Screenshot |
|------------|-------------|------------------|
| [M0001-fix-NamedObjectContext-nullptr-crash.patch](M0001-fix-NamedObjectContext-nullptr-crash.patch) (Playerbots) | Fixes a potential crash when NamedObjectContext::create() returns a null pointer | [1️⃣ View](images/Namedobjectcontect_M0001_1.png)<br>[2️⃣ View](images/Namedobjectcontect_M0001_2.png) |

## 💡 Usage

```bash
cd /opt/cmangos/mangos
git apply /opt/cmangos/mangos/patches/modules/M0001-fix-NamedObjectContext-nullptr-crash.patch

