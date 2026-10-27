# Port Map

Network port map for rack cabinets: switch port → patch panel port → floor / room → device.
Installable web app (PWA) that also works offline.

Version 3.1 adds:
- Separate **IP** and **MAC** fields (the old “name / IP / MAC” text is split automatically once; a browser copy of the 3.0 data is kept as `portmap-store-v2.backup-3.0`).
- Switch port settings: access / trunk (802.1Q), native VLAN, allowed VLANs, speed, PoE class (802.3af/at/bt), enabled / shutdown.
- Cable ID and a TIA-606 style position label (`Rack-Panel-Port`).
- Checks: duplicate IP / MAC / cable ID, invalid IP / MAC, IP outside its VLAN subnet, trunk VLANs not in the VLAN list, native VLAN / speed / mode mismatch at the two ends of a link.
- **CSV / Excel** export of all connections and **Print / PDF**.

- Data is stored only on the device that uses it (browser storage). Nothing is uploaded.
- Move data between devices with **Export / Import** (`.portmap.json`).
- Languages: English, Русский, Türkçe, Azərbaycanca.

Open the app: https://ulveelives.github.io/portmap/
