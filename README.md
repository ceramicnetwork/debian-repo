# ceramicnetwork package repo

## Install

Add the package repository key to your system
```
curl -fsSL https://ceramicnetwork.github.io/repo/public_key.gpg | sudo gpg --dearmor -o /usr/share/keyrings/ceramic-network-archive-keyring.gpg
```

Add the package repository to your system
```
echo "deb [signed-by=/usr/share/keyrings/ceramic-network-archive-keyring.gpg] https://ceramicnetwork.github.io/repo stable main " | sudo tee /etc/apt/sources.list.d/ceramicnetwork.list
```

Update the package cache
```
sudo apt update
```

Install the package
```
sudo apt install -y ceramic-one
```
