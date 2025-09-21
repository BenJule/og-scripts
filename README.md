# Resource Distribution Script (ANK-Compatible)

🚀 **Automatic Resource Distribution for OGame**

---

## Description

This script automatically distributes resources between all your planets and moons in OGame.
It is **100% ANK-compatible** and provides **German logs with icons** for clear tracking of all transfers.

* Supports **Metal, Crystal, and Deuterium**
* Uses **all ship types** for transport
* Automatic **resource splitting** across all planets
* Takes **fleet capacity and free slots** into account
* **Rounds resource amounts** to configurable units

---

## Features

* 📦 Automatic transfer of resources between planets
* ⏳ Waits if no fleet slots are available
* ⚠️ Handles errors when transport capacity is insufficient
* 🔄 Dynamically calculates resource needs per planet
* 🚀 Supports **all ship types** (Small/Large Cargo, Reaper, Battlecruiser, Bomber, Destroyer, Pathfinder)
* 📝 German logs with icons for easy tracking

---

## Configuration

```javascript
splitPlanetWorkers = "allPlanets" // or array ["M:1:2:4", "P:2:3:4"]
splitMetal       = true           // split Metal
splitCrystal     = true           // split Crystal
splitDeuterium   = true           // split Deuterium
roundFactor      = 500000         // rounding factor for resources
```

* `splitPlanetWorkers`: `"allPlanets"` for all planets/moons or a specific list
* `splitMetal`, `splitCrystal`, `splitDeuterium`: select which resources to distribute
* `roundFactor`: rounds resource amounts to multiples of this number (e.g., 500,000)

---

## Usage

1. Import the script into ANK/NinjaBot
2. Adjust the configuration as needed
3. Run the script: `doWork()`
4. The script automatically logs all transfers and status messages in the console

---

## Notes

* Make sure there are enough **free fleet slots** available
* Adjust the rounding factor to distribute **exact amounts**
* Logs are in **German with icons** for better readability
* Works on **all planets and moons** recognized by ANK

---

## License

This script is free to use for private purposes. Commercial use only with permission.
