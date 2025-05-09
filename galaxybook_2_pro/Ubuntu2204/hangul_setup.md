```bash
sudo apt update
```
```bash
sudo apt install fcitx5 fcitx5-hangul fcitx5-frontend-gtk3 fcitx5-frontend-qt5 fcitx5-config-qt
```

```bash
mkdir -p ~/.config/environment.d
```

```bash
cat <<EOF > ~/.config/environment.d/fcitx5.conf
GTK_IM_MODULE=fcitx
QT_IM_MODULE=fcitx
XMODIFIERS="@im=fcitx"
INPUT_METHOD=fcitx
SDL_IM_MODULE=fcitx
GLFW_IM_MODULE=ibus
EOF
```

```bash
fcitx5-config-qt
```
```bash
im-config
```