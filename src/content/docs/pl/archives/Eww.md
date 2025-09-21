---
title: Eww (wiele)
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
Kilka zestawów konfiguracji, w tym `windoes`, `hybrid`, `NovelKnock`, itp.
# Instalacja
- Zależności: Zobacz listę zależności do specyficznej gałęzi
- Skopiuj te elementy
    - `.config`, `.local` do swojego katalogu domowego
    - Foldery z `.local/share/icons` do `/usr/share/icons`
    - Pliki z folderu `Import manually`, jeśli są potrzebne

 ## Wydajność
|  ⌄  | Używaj | Nie rekomendowane | Notatki                 |
| --- | ------ | ----------- | ------------------------- |
| Jądro |     | cachyos, xanmod | Nie nadużywaj funkcji oszczędzania energii. Poza tym nie jestem pewien, co do cholery mówię – to tylko moje osobiste doświadczenie. |
| Powłoka logowania  | bash/zsh | fish | To ok aby używać fish w terminalu - tak robi end_4 |

 ## Konfiguracja
 - Konfiguracje eww działają poprawnie tylko w `~/.config/eww`
 - Uruchom eww za pomocą `eww daemon`
 - Aby otworzyć pasek górny: `eww open bar`
 - Aby otworzyć pasek Windows: `eww open winbar` (gałąź `windoes`/`hybrid`)
 - Aby otworzyć linię dolną: `eww open bottomline` (tak aby okienko muzyki otwierało się kiedy klikniej dolny róg ekranu)
 - Otwórz widok ogólny (kliknij środkowym przyciskiem myszy przestrzenie robocze) i poczekaj 10 sekund (aby wygenerować pamięć podręczną wyszukiwania aplikacji, inaczej ikony nie będą wyświetlane poprawnie.)
 ## Używanie
- Sterowanie muzuką: kliknij środkowym przyciskiem myszy aby odtwarzać/wstrzymać, kliknij prawym aby odtworzyć następny utwór, przewijaj aby zmienić głośność
- Aby otworzyć widok ogólny, kliknij środkowym lub prawym przyciskiem myszy wskaźniki przestrzeni roboczych lub uruchom `eww open overview`
- W widoku ogólnym wpisuj, aby wyszukać aplikacje (zobacz poniżej)

## Wyszukiwanie
- Wpisuj, aby wyszukać aplikacje  
- Wpisz wyrażenie matematyczne (musi zaczynać się od cyfry), aby obliczyć za pomocą qalc
- `>save MOTYW`: Zapisuje aktualny motyw pod nazwą MOTYW
- `>load MOTYW`: Wczytuje zapisany motyw. Dostępne motyw będą podpowiadane podczas wpisywania
- `>music`: Pobiera motyw z aktualnej miniaturki utworu
- `>wall`: Pobiera motyw z tapety znajdującej się w `~/.config/eww/images/wallpaper/wallpaper`
- `>light`: Pamiętaj, aby używać trybu jasnego przy kolejnych generacjach kolorów
- `>dark`: Pamiętaj, aby używać trybu ciemnego przy kolejnych generacjach kolorów
- `>one`: Pamiętaj, aby używać tylko jednego koloru dla ikon paska przy kolejnych generacjach kolorów
- `>multi`: Pamiętaj, aby używać wielu kolorów dla ikon paska przy kolejnych generacjach kolorów
- `>r`: Uruchom ponownie (zabija i ponownie uruchamia eww z domyślnym paskiem)
