# Voron V2.4 – Blue Printer Configuration

This repository contains the full Klipper configuration for my **Voron V2.4** printer (nicknamed **Blue**).

This configuration includes several custom macro systems designed to make multi-print workflows much faster while still maintaining safety.

## Key Features

- Hot Standby Mode
- Fast Restart (skip homing and QGL)
- TAP sanity probe validation
- Automatic standby timeout shutdown
- Chamber air purge safety cycle
- MMU-friendly print ending
- Material-aware fan behavior

---

# Printer Hardware

| Component | Details |
|---|---|
| Printer | Voron V2.4 |
| Probe | Voron TAP |
| Toolhead | TAP compatible |
| MMU | ERCF |
| Chamber | Fully enclosed |
| Filtration | Nevermore |
| Airflow | Intake / Exhaust / Cooling fans |
| Firmware | Klipper |

---

# Major Macro Systems

## Hot Standby Mode

Hot standby allows the printer to remain in a **ready-to-print state** after a print finishes.

This is intended for workflows where multiple prints are started in sequence using the same material.

Hot standby is controlled with:
