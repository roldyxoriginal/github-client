# Github Client

#### Instalacion

* Descargamos el cliente binario desde la pagina de github, buscando en mi caso el archivo .deb
* Luego
```
sudo apt install ./gh_2.0.0_linux_amd64.deb
```

#### Login en github
```
gh auth login
```
* Utilizamos el mecanismo de ssh (hay que poner la clave publica en el destino)

#### Primer commit
```
git init
gh repo create --public
git add .
git commit -m "Commit Inicial"
git push --set-upstream origin main


```

