# Neutrine Debian Repository

## Setup

1. Trust key
```bash
sudo wget -q "https://neutrine.com/deb/public.gpg" -O /etc/apt/trusted.gpg.d/neutrine.com.gpg
```

2. Add APT repository

### bullseye
```bash
sudo sh -c 'echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/trusted.gpg.d/neutrine.com.gpg] https://deb.neutrine.com bullseye main" > /etc/apt/sources.list.d/neutrine.com.list'
```

### buster
```bash
sudo sh -c 'echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/trusted.gpg.d/neutrine.com.gpg] https://deb.neutrine.com bullseye main" > /etc/apt/sources.list.d/neutrine.com.list'
```

3. APT update
```bash
sudo apt update
```
