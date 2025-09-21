---
title: m3ww
layout: /src/layouts/autonum.astro
sidebar:
  badge:
    text: !TODODeprecated
    variant: !TODOcaution
lastUpdated: !TODO2024-02-18
---

:::danger[Niebezpieczeństwo]
Ten zestaw konfiguracji nie jest już utrzymywany. Zalecamy, aby go nie używać.
:::

# Opis
- Najnowsza konfiguracja oparta na Eww, która naśladuje styl [Material Design 3](https://m3.material.io/)

# Instalacja
- Zainstaluj zależności i dodaj użytkownika do grupy `video`

```bash
# Normalne pakiety
sudo pacman -S bc blueberry bluez boost boost-libs cliphist coreutils curl findutils fish fuzzel fzf gawk gnome-control-center gnome-keyring grim ibus imagemagick libqalculate light networkmanager network-manager-applet nlohmann-json pavucontrol plasma-browser-integration playerctl procps polkit-gnome ripgrep slurp socat sox starship udev upower util-linux xorg-xrandr wget wireplumber yad tesseract
# Pakiety AUR - instalacja za pomocą yay
yay -S cava eww-tray-wayland-git geticons gojq gtklock gtklock-playerctl-module gtklock-powerbar-module gtklock-userinfo-module hyprland-git lexend-fonts-git python-material-color-utilities python-pywal python-desktop-entry-lib python-poetry python-build python-pillow swww ttf-material-symbols-git wlogout
# Dodaj użytkownika do grupy `video`
sudo usermod -aG video $(whoami)
```

- Skopiuj te elementy
    - `.config`, `.local` do swojego katalogu domowego
    - Foldery z `.local/share/icons` do `/usr/share/icons`
    - Pliki z folderu `Import manually`, jeśli są potrzebne

- Opcjonalne
   - Uwaga: Jeśli nie potrzebujesz wielu układów klawiatury, zakomentuj wszystko związane z ibus w `~/.config/hypr/execs.conf`. Jeśli jednak potrzebujesz, możesz użyć fcitx5 (choć nie będzie on zintegrowany z ikoną na pasku).
   - Jeśli chcesz, aby miniatury multimediów z przeglądarki były wyświetlane, zainstaluj rozszerzenie "Plasma browser integration":
     - Dla [Chromium](https://chrome.google.com/webstore/detail/plasma-integration/cimiefiiaegbelhefglklhhakcgmhkai)
     - Dla [Firefox](https://addons.mozilla.org/en-US/firefox/addon/plasma-integration/)

