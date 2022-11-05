# Neutrine Debian Repository

## Setup

1. Add package signing key and repository:
```bash
curl -fsSL https://neutrine.com/deb/public.gpg | sudo tee /etc/apt/trusted.gpg.d/neutrine.com.gpg >/dev/null
sudo sh -c 'echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/trusted.gpg.d/neutrine.com.gpg] https://deb.neutrine.com bullseye main" > /etc/apt/sources.list.d/neutrine.com.list'
```

2. Install package:
```bash
sudo apt-get update
sudo apt-get install <package-name>
```
