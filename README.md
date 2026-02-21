# EZupnp

A simple command line tool to manage port forwarding on your router via UPnP.

## Requirements

- Python 3
- `miniupnpc` (will be offered for installation on first run if missing)

## Usage

```
# Open a TCP port
./ezupnp -o 8080

# Open a UDP port
./ezupnp -o 8080 -u

# Open a port with a 1-hour lease
./ezupnp -o 8080 -d 3600

# Close a TCP port
./ezupnp -c 8080

# Close a UDP port
./ezupnp -c 8080 -u

# List all port mappings
./ezupnp -l

# Show gateway status
./ezupnp -s

# Show traffic statistics
./ezupnp -t
```

## Options

| Flag | Description |
|------|-------------|
| `-o PORT` | Open/forward a port |
| `-c PORT` | Close a port mapping |
| `-l` | List all port mappings |
| `-s` | Show gateway status (IPs, uptime, connection info) |
| `-t` | Show traffic statistics (bytes/packets sent/received) |
| `-u` | Use UDP instead of TCP (for `-o` and `-c`) |
| `-d SEC` | Lease duration in seconds, 0 = indefinite (default: 0) |
