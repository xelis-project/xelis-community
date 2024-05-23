# Mining Hashrates

This folder contains the a `hashrate.js` file.
You can add your device mining information in there.

The format explained:

- Date: Add the date of your entry
- Type: CPU or GPU
- Brand: Brand of the device. Ex: NVIDIA
- Model: Model of the device. Ex: RTX 4070 Ti
- Miner: The mining software used. Ex: Rigel v1.17.2
- User: Your username. Leave empty if you want.
- Stock (no modifications)
  - Hashrate: Actual hashrate reported in (kh/s).
  - Power Range: The power draw range in watts. Ex: [140, 160]
- OC (overclock)
  - Core Clock: The core clock in Ghz.
  - Core Clock Offset: The core clock offset.
  - Mem Clock: The memory clock in Ghz.
  - Mem Clock Offset: The memory clock offset.
  - Hashrate: Actual hashrate reported in (kh/s).
  - Power Range: The power draw range in watts. Ex: [140, 160]
- MAX OC (maximum overclock)
  - Core Clock: The core clock in Ghz.
  - Core Clock Offset: The core clock offset.
  - Mem Clock: The memory clock in Ghz.
  - Mem Clock Offset: The memory clock offset.
  - Hashrate: Actual hashrate reported in (kh/s).
  - Power Range: The power draw range in watts. Ex: [140, 160]

We don't store efficiency because we can calculate with `hashrate (KH/s) / power consumption (watts)`.

You can copy this default template and modify the values.
Paste in the array inside `hashrate.js` afterwards:

```js
  {
    "date": "",
    "type": "",
    "brand": "",
    "model": "",
    "miner": "",
    "user": "",
    "stock": {
      "hashrate": 0,
      "power_range": [0, 0],
    },
    "oc": {
      "core_clock": 0,
      "core_clock_offset": 0,
      "mem_clock_offset": 0,
      "mem_clock": 0,
      "hashrate": 0,
      "power_range": [0, 0]
    },
    "max_oc": {
      "core_clock": 0,
      "core_clock_offset": 0,
      "mem_clock_offset": 0,
      "mem_clock": 0,
      "hashrate": 0,
      "power_range": [0, 0]
    }
  }
```

If you don't want to create an Github account and a Pull request. Paste this populated value in the Discord and someone can add on your behalf.
