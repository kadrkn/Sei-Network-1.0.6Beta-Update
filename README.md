# Sei-Network-1.0.6Beta-Update
Sei Network Atlantic-1 Testnet 1.0.6 Beta Güncellemesi

Exit-Code hatası alan arkadaşlarda bu komutları deneyebilir. Bende aynı sorun vardı, bu komutlarla sorun giderildi. 

```
cd $HOME
```

```
sudo rm sei-chain -rf
```

```
git clone https://github.com/sei-protocol/sei-chain.git
```

```
cd sei-chain
```

```
sudo systemctl stop seid
```

```
git checkout master && git pull
```

```
git checkout 1.0.6beta-val-count-fix
```

```
make install
```

```
sudo cp /root/go/bin/seid /usr/local/bin/seid
```

```
sudo systemctl restart seid
```

```
sudo journalctl -u seid -f -o cat
```
