# MAC Changer

A Python tool that changes the MAC address of a network interface on Linux. Updated to Python 3.

> **Disclaimer:** For educational purposes and authorized testing only. Only use on your own devices. The author is not responsible for any misuse.

---

## How it works

1. Takes a network interface name and desired MAC address as arguments
2. Brings the interface down
3. Sets the new MAC address via `ifconfig`
4. Brings the interface back up
5. Verifies the change was applied successfully

## Requirements

Python 3 standard library only — no additional packages needed.

> **Note:** Linux only. Requires root privileges (`sudo`).

## Usage

```bash
sudo python3 mac_changer.py -i <interface> -m <new_mac>
```

```bash
sudo python3 mac_changer.py -i eth0 -m 00:11:22:33:44:55
```

To find your interface name:

```bash
ifconfig -a
```

Use `--help` for all options.

---

## Part of [H-Tools](https://github.com/shubham-patel/H-Tools)

Built during B.Tech studies. H-Tools bundles this and other networking/security utilities in a single CLI menu.
