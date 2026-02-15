# EZupnp

A simple command line tool to manage port forwarding on your router via UPnP.

## Requirements

- Python 3
- `miniupnpc` (will be offered for installation on first run if missing)

## Usage

```
# Open a port
./ezupnp -o 8080

# Close a port
./ezupnp -c 8080

# List all port mappings
./ezupnp -l
```
