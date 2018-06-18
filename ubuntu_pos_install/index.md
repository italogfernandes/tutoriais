# Ubuntu 18.04 - Pós Instalação


## Pós instalação

Referências:
* http://www.edivaldobrito.com.br/dicas-de-coisas-para-fazer-ubuntu-16-04/
* https://www.diolinux.com.br/2016/04/7-coisas-para-fazer-depois-de-instalar-o-ubuntu-1604-lts.html
* https://www.diolinux.com.br/2018/04/o-que-fazer-depois-instalar-ubuntu-1804-lts.html
* http://www.edivaldobrito.com.br/coisas-para-fazer-depois-de-instalar-o-ubuntu-18-04-lts/

### Atualizando o sistema
Adicionar parceitos da canonical
```bash
# Atualizar os repositorios
sudo apt-get update
# Atualizar os programas
sudo apt-get upgrade
```


### Completar instalação de idiomas
Via interface, ir ate idiomas.

### Drivers
Verifique os drivers

### Alguns softwares uteis

```bash
sudo apt-get install gdebi bleachbit ubuntu-restricted-extras
```

### Outros
```bash
sudo apt-get install gdebi vlc
```


### Configurações
* Wallpaper
* Contas online
* Templates

### Temas
```bash
sudo apt-get install gnome-tweak-tool 
# Paper icon theme
sudo add-apt-repository ppa:snwh/pulp -y && sudo apt-get update && sudo apt-get install paper-icon-theme -y
```

```bash
gsettings set org.gnome.desktop.wm.preferences button-layout 'close,maximize,minimize:'
```

* https://addons.mozilla.org/en/firefox/addon/gnome-shell-integration/
* https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep
```bash
sudo apt install chrome-gnome-shell
```


Ativando repositorios parceiros
```bash
#TODO
```

## Instalando todos os programas

### General Codding Tools

* Atom
* Sublime Text
* Git
* Git Kraken

#### Atom
Referência: https://flight-manual.atom.io/getting-started/sections/installing-atom/#platform-linux
**Instalando**
```bash
curl -sL https://packagecloud.io/AtomEditor/atom/gpgkey | sudo apt-key add -
sudo sh -c 'echo "deb [arch=amd64] https://packagecloud.io/AtomEditor/atom/any/ any main" > /etc/apt/sources.list.d/atom.list'
sudo apt-get update
sudo apt-get install atom
```
**Configurando**: Copie a pasta .atom da instalação anterior

#### Sublime Text
Referência: https://www.sublimetext.com/docs/3/linux_repositories.html
**Instalando**
```bash
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
sudo apt-get install apt-transport-https
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```

#### Git

**Instalando**
```bash
sudo apt-get install git
```
**Configurando**: 
* Git: 
```bash
git config --global user.name "Ítalo Fernandes"
git config --global user.email "italogsfernandes@gmail.com"
```
* SSH + GitHub
Referências: https://help.github.com/articles/connecting-to-github-with-ssh/
```bash
ssh-keygen -t rsa -b 4096 -C "italogsfernandes@gmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
sudo apt-get install xclip
# Downloads and installs xclip. If you don't have `apt-get`, you might need to use another installer (like `yum`)
xclip -sel clip < ~/.ssh/id_rsa.pub
# Copies the contents of the id_rsa.pub file to your clipboard
```
* Clonando all the repos
```bash
mkdir ~/Documents/GitHub/
#TODO: Comando para clonar tudo
```

#### GitKraken

**Instalando**
```bash
sudo apt-get install git
```

### IDEs

#### Anaconda
```bash
# Anaconda
bash ~/Téléchargements/Anaconda3-5.1.0-Linux-x86_64.sh
sudo desktop-file-install spyder.desktop 
sudo desktop-file-install anaconda.desktop 

bash ~/Téléchargements/Anaconda3-5.1.0-Linux-x86_64.sh 
anaconda-navigator
sudo desktop-file-install anaconda.desktop 
cd /opt
mkdir anaconda
cd anaconda/
sudo desktop-file-install spyder.desktop 
conda update --all
conda update spyder
export PATH=~/anaconda3/bin:$PATH
conda update spyder
conda update -n base conda
conda update spyder
spyder
cd ~/PG/anaconda/
spyder
cd ~/PG/
cd anaconda/
ls
nano spyder.desktop 
sudo desktop-file-install spyder.desktop 
spyder %F
spyder
cd ~
spyder
conda
conda update --all
```

#### Matlab
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

### Apps

#### Telegram
https://desktop.telegram.org/

#### Skype


#### Unified Remote


### Embedded Systems

#### Arduino

#### Platomformio

### Electronics

### Eagle
```bash
./install-desktop-icon.sh 
ls
chmod -x install-desktop-icon.sh 
ls
./install-desktop-icon.sh
sudo ./install-desktop-icon.sh
cd ..
ls
sudo desktop-file-install eagle.desktop 
sudo desktop-file-validate eagle.desktop 
sudo desktop-file-install eagle.desktop 
```
### Qucs

### DraftSight

###
```bash
sudo apt-get install apache2
```

## XFCE4

Instalando
```bash
sudo apt-get install xfce4
```

Logue, e deslogue, é preciso configurar a aparencia e etc...

Varios applets:
```bash
sudo apt-get install xfce4-weather-plugin 
sudo apt-get install xfce4-weather-plugin xfce4-wmdock-plugin 
sudo apt-get install xfce4-battery-plugin
sudo apt-get install xfce4-windowck-plugin
sudo apt-get install xfce4-appmenu-plugin 
sudo apt-get install xfce4-whiskermenu-plugin 
```

As vezes eu nao faço ideia do que aconteceu
```bash
applications-menu
menulibre
```

```bash
exo-open --launch whiskermenu
exo-open --launch WhiskerMenu
whiskermenu
whisker
```

Configurando o atalho para o botão super
```bash
xcfe4-popup-applicationsmenu
xcfe4-whiskermenu-plugin
xcfe4-whiskermenu
xcfe4-popup-whiskermenu
xcfe4-popup-whisker
```

Alguns applets foram instalados do modo raiz:
Não lembro quais, mas aqui ta o qe eu fiz -q
```bash
sudo gdebi xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
sudo apt-get install libxfce4util
sudo apt-get install libxfce4util-dev
sudo gdebi xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
sudo apt-get install libxfce4util7
sudo apt-get install libxfce4util6
udo apt-get install autotools-dev pkg-config intltool dh-autoreconf libgtk2.0-dev xfce4-dev-tools xfce4-panel-dev libxfce4util-dev libxfconf-0-dev libxfce4ui-1-dev libwnck-dev wget
sudo apt-get install autotools-dev pkg-config intltool dh-autoreconf libgtk2.0-dev xfce4-dev-tools xfce4-panel-dev libxfce4util-dev libxfconf-0-dev libxfce4ui-1-dev libwnck-dev wget
sudo gdebi xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
nano xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
sudo gdebi -f xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
sudo gdebi --force xfce4-windowck-plugin_0.3.0-0~eugenesan~utopic4_amd64.deb 
sudo add-apt-repository ppa:oiteam/xfce4
sudo add-apt-repository --remove ppa:oiteam/xfce4
sudo apt-get update
cd xfce4-windowck-plugin-0.4.4/
./autogen.sh --prefix=/usr
make
sudo make install
ls
unzip xfce4-netspeed-plugin-master.zip 
ls
cd xfce4-netspeed-plugin-master/
ls
./configure
./autogen.sh
cd ..
sudo chmod -R +x xfce4-netspeed-plugin-master/
ls
cd xfce4-netspeed-plugin-master/
ls
./configure
./autogen.sh 
make
./autogen.sh --prefix=/usr
make
ls
./configure
make
ls
cat install-sh 
./install-sh 
ls
make
sudo make install
cat INSTALL 
ls
./configure
sudo apt-get install libgtop
sudo apt-get install libgtop-2.0-11 
sudo apt-get install libgtop2-common 
sudo apt-get install libgtop2-dev
./configure
make
sudo make install
ls
sudo apt-get install libxfce4util
sudo apt-get install libxfce4util-dev
sudo apt-get install libxfce4ui
sudo apt-get install libxfce4ui-common 
sudo apt-get install libxfce4ui-utils 
sudo apt-get install libxfce4ui
sudo apt-get install libxfce4ui-1-0
sudo apt-get install libxfce4ui-2
sudo apt-get install libxfce4ui-2-0 
sudo apt-get install libxfce4ui-2-0-deve
sudo apt-get install libxfce4ui-2-0-dev
sudo apt-get install libxfce4ui-2-dev
./configure && make && sudo make instal
./configure --prefix=/usr && make && sudo make instal
sudo apt-get install intltool xfce4-dev-tools libxfce4util-dev libgtk2.0-dev libxfcegui4-dev libxfce4util-dev xfce4-panel-dev libgtop2-dev
./configure --prefix=/usr && make && sudo make install
```

Algum desses comandos foi responsavel por ativar o clique com o touchpad no xfce4
```bash
xinput list-props "SynPS/2 Synaptics TouchPad"
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/Synaptics_Coasting_Speed -n -t double -s 0
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/Synaptics_Scrolling_Distance -n -t int -t int -s 50 -s 80
xinput list-props "SynPS/2 Synaptics TouchPad"
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput Tapping Enabled -n -t int -s 1
xinput list-props "SynPS/2 Synaptics TouchPad"
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput Tapping Enabled -n -t bool -s 1
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput Tapping Enabled -n -t gboolean -s 1
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput Tapping Enabled -n -t int -s 1
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput_Tapping_Enabled -n -t int -s 1
xinput list-props "SynPS/2 Synaptics TouchPad"
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput_Tapping_Enabled_Default -n -t int -s 1
xinput list-props "SynPS/2 Synaptics TouchPad"
xfconf-query -c pointers -p /SynPS2_Synaptics_TouchPad/Properties/libinput_Tapping_Enabled_Default -n -t int -s 1
xinput list-props "SynPS/2 Synaptics TouchPad"
sudo apt-get install gpointing-device-settings
xinput list-props "SynPS/2 Synaptics TouchPad"
```

Desativando o bluetooth
```bash
rfkill block bluetooth
```

Desativando as mensagens de erro constantes
```bash
sudo nano /etc/default/apport
sudo service apport stop
```

Atalhos para screenshots
```bash
gnome-screenshot --interactive
gnome-screenshot
gnome-screenshot --h
gnome-screenshot -h
gnome-screenshot -c
```

Alterando configurações do usuario
```bash
sudo apt-get install mugshot 
```

Applet de controle de brilho (lembre-se de add ele no painel após instalar):
```bash
sudo apt-get install xfce4-power-manager
sudo apt-get install xfce4-brightness-plugin
```

Troque o gerenciador de arquivos default para o nautilus, teste com:
```bash
exo-open --launch=FileManager
```