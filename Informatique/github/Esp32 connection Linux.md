# Comment faire en sorte que cela fonctionne à chaque fois

## Arch Linux 
- Ajouter son utilisateur au groupe `uucp`
```
sudo usermod -a -G uucp $USER
```


## Ubuntu
- Ajouter son utilisateur au groupe `dialout`
```
sudo usermod -a -G dialout $USER
```
- Et **surtout**, désinstaller `brltty` (merci à [reddit](https://askubuntu.com/questions/1403705/dev-ttyusb0-not-present-in-ubuntu-22-04))
```
sudo apt remove brltty
```
