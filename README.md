# cmangos-crash-module-debug

Patch collection to fix crashes and stability issues in CMaNGOS modules (e.g., PlayerBots, TrainingDummies, etc.)

## 🛠️ Included Patches

| Patch File | Description | Crash Screenshot |
|------------|-------------|------------------|
| [0001-fix-ObjectGridLoaderxx-LoadHelper-crash.patch](0001-fix-ObjectGridLoaderxx-LoadHelper-crash.patch) | xxFixes a potential crash in `LoadHelper` caused by `IsInWorld()` assertion failure | [1️⃣ View](xximages/Objektgridloadererror_0001_1.png)<br>[2️⃣ View](xximages/Objektgridloadererror_0001_2.png) |

## 💡 Usage

```bash
cd /opt/cmangos/mangos
git apply /opt/cmangos/mangos/patches/modules/M0001-fix-PlayerBot-UpdateInternal-crash.patch

