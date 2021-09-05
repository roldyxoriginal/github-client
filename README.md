# Github Client

#### Instalacion

* Descargamos el cliente binario desde la pagina de github, buscando en mi caso el archivo .deb
```
sudo apt install ./gh_2.0.0_linux_amd64.deb
```

#### Login en github
```
gh auth login
```
* Utilizamos el mecanismo de ssh (hay que poner la clave pública(id_rsa.pub) en el destino(github))

#### Para que se utilice main y no master (Black Lives Matter)
```
mkdir ~/.git-template
echo "ref: refs/heads/main" >>~/.git-template/HEAD
git config --global init.templateDir ~/.git-template
```

#### Primer commit
```
git init
gh repo create --public
git add .
git commit -m "Commit Inicial"
git push --set-upstream origin master
```

#### Para realizar un fork
```
gh repo fork https://github.com/learn-devops-fast/spock-lizard-docker.git --clone
```
