# Ubuntu 18.04 - Pós Instalação


## Primeiro de Tudo

Atualizando o sistema
```bash
# Atualizar os repositorios
sudo apt-get update
# Atualizar os programas
sudo apt-get upgrade
```

Ativando repositorios parceiros
```bash
#TODO
```

## Instalando todos os programas

### Da central de software
```bash
# Gdebi
sudo apt-get install gdebi

# Gnome Tweak-Tool
sudo apt-get install gnome-tweak-get install gnome-tweak

# Paper icon theme
sudo add-apt-repository ppa:snwh/pulp -y && sudo apt-get update && sudo apt-get install paper-icon-theme -y

# Git
sudo apt-get install git

# Eagle
sudo apt-get install eagle
```

### Via snap

```


```
### Via ppa
```bash

```

### Via .deb arquivo baixado
```


```

### Via outros tipos de arquivos baixados
```bash
# Anaconda
bash ~/Téléchargements/Anaconda3-5.1.0-Linux-x86_64.sh
```

### Complicados
```bash

# Matlab
mkdir matlab_tmp
ls
cd /media/italo/MATHWORKS_R2018A
ls
sudo rm -rf /usr/local/MATLAB/R2018a/
./install
cd ..
ls
sudo chmod -R 777 matlab_tmp/
cd matlab_tmp/
./install
cd ~
./PG/matlab_tmp/install
sudo ./PG/matlab_tmp/install
sudo ./media/italo/MATHWORKS_R2018A/install
./media/italo/MATHWORKS_R2018A/install
sudo chmod -R 777 matlab_tmp/
sudo chmod -R 777 /PG/matlab_tmp/
sudo chmod -R 777 PG/matlab_tmp/
./media/italo/MATHWORKS_R2018A/install
./PG/matlab_tmp/install
sudo ./PG/matlab_tmp/install
sudo chmod -R 777 PG/matlab_tmp/
sudo ./PG/matlab_tmp/install
sudo rm -rf matlab_tmp/
sudo chmod -R 777 /usr/local/MATLAB/R2018a/
sudo ./usr/local/MATLAB/R2018a/bin/matlab
cd /usr/local/MATLAB/R2018a/bin/
sudo ./matlab
sudo apt-get install matlab
sudo apt-get install matlab-support
sudo /media/italo/MATHWORKS_R2018A/install &
sudo /media/italo/MATHWORKS_R2018A/install
cp R2018a/ /usr/local/MATLAB/R2018a/
cp -r R2018a/ /usr/local/MATLAB/R2018a/
sudo cp -r R2018a/ /usr/local/MATLAB/R2018a/
```
## Configurando

```bash
# Git
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
sudo apt-get install xclip
xclip -sel clip < ~/.ssh/id_rsa.pub
```
## Gnome TweakTool
