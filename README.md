#### Build

From [building-pfsense-iso-from-source](https://github.com/Augustin-FL/building-pfsense-iso-from-source)

```
pkg install -y git
```

```
git clone https://github.com/mola/pfsense-builder.git
cd pfsense-builder
chmod +x *.sh
```

```
./install_dep.sh
./sign_setup.sh
./clone_repo.sh
```
```
cd /root/pfscense
screen -S build
./build.sh --setup-poudriere
```
