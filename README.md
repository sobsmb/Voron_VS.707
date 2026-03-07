# Voron VS.707 – Enderwire Configuration

Configuration repository for **Voron VS.707**, an **Enderwire conversion** running Klipper.

This repository contains the printer configuration, macros, and supporting service configuration.

---

## Printer Details

| Component | Description               |
| --------- | ------------------------- |
| Printer   | Enderwire                 |
| Firmware  | Klipper                   |
| Host      | Raspberry Pi (MainsailOS) |
| UI        | Mainsail / KlipperScreen  |

---

## Repository Layout

```
printer.cfg                Main Klipper entrypoint

hardware/                  Hardware configuration
features/                  Optional printer features
tuning/                    Input shaper / accelerometer tuning

macros/                    Organized macros
services/                  Host-side service configs

archive/                   Old configs retained for reference
artifacts/                 Runtime files ignored by git
```

---

## Configuration Backup

The repository includes a macro to automatically back up configuration changes.

Run:

```
BACKUP_CFG
```

This executes:

```
services/autocommit.sh
```

which commits and pushes configuration changes to GitHub.

---

## Notes

* Runtime files are ignored via `.gitignore`
* Configuration structure is shared across printers for consistency
* Designed for easy cloning and reuse

---

## License

MIT License

---

## Author

Jason S
