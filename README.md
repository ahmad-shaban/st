# **Custom build of st terminal from [suckless.org](http://st.suckless.org) by A7MED**

---
## **Applied patches**
* #### scrollback-ringbuffer
* #### scrollback-mouse
* #### scrollback-mouse-altscreen
* #### alpha
* #### anygeometry
* #### anysize
* #### workingdir
* #### delkey
* #### nano shortcuts support
* #### font2
* #### defaultfontsize
* #### vertcenter
* #### blinkingcursor

* ### I also added a custom colorscheme
* ### Used fonts are `Hack` and `Symbola`

---
## **How to build**
### **Install dependencies**
* #### **Debian**
  ```bash
  sudo apt install libx11-dev libxft-dev
  ```
* #### **Fedora**
  ```bash
  sudo dnf install libx11-devel libxft-devel
  ```
* #### **Arch**
  ```bash
  sudo pacman -S libx11 libxft
  ```
  
### Clone the repo and start building
```bash
git clone https://github.com/ahmed0124/st.git
cd st
sudo make clean install
```

Now it should be installed on your system and you can run it from command line. You may want to write a st.desktop file and put it on `/usr/share/applications` to make st appear in your applications menu. Here is an examble of the contents of that file
```
[Desktop Entry]
Name=st
Comment=simple terminal emulator from suckless.org
Type=Application
Categories=Utility;
Terminal=false
Icon=terminal
Exec=st
```
if it still don't appear on your apps menu, restart your pc and it should appear
