# nomadcap

PCAP tool that aids in locating misconfigured network stacks

## Build

Install build essentials and PCAP library with headers.

```bash
sudo apt update
sudo apt install build-essential libpcap0.8 libpcap-dev
```

Run `make` to compile. Results are in the directory `build/`.

## Usage

Run `nomadcap` with Root privileges or through `sudo`.

```bash
sudo build/nomadcap -v
```

Output should list devices with network stacks misconfigured that
are sending ARP requests for other networks.