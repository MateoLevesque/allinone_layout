# Allinone keyboard layout.

This is a custom xkb layout based on the QWERTY US layout that includes easy access to French, German, Norwegian and Spanish characters.

# The layout
This layout is layer-based so to use the new characters you need to press `alt-gr + e` for the symbol `é` for example.

I use this layout on hyprland and didn't test it on other system. Also, all the letters are placed to satisfy my own likings. Feel free to adapt them to yours.

![layout visual](https://github.com/MateoLevesque/allinone_layout/blob/main/keyboard-layout.png?raw=true)

# Installation

Clone the repository: 

```{bash}
git clone https://github.com/MateoLevesque/allinone_layout.git
cd allinone-layout
```


Add the layout to your layout directory: 

```{bash}
sudo cp allinone /usr/share/X11/xkb/symbols/
```

Edit your hyprland config file (usually at ~/.config/hypr/input.conf) to add the following lines:

```{lua}
input {
    kb_layout = allinone
    kb_options = lv3:ralt_switch
}
```

