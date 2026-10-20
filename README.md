# Wallpapers

Pixel art wallpapers cho Windows Terminal va Start menu (Windows 11).

Anh cua `cat-bg.gif` la GIF dong (1920x1080, 49 frame) - dung lam nen cho
Windows Terminal, chi chay o tab dang focus.

## Dung trong Windows Terminal

```json
"backgroundImage": "https://raw.githubusercontent.com/kh4i-dev/wallpapers/main/cat-bg.gif",
"backgroundImageOpacity": 0.35,
"backgroundImageAlignment": "center",
"backgroundImageStretchMode": "uniformToFill"
```

## Dung trong Start menu (Windows 11)

Start menu khong cho dat anh nen truc tiep. Can Windhawk + mod
*Windows 11 Start Menu Styler*:

```json
{
  "controlStyles[0].target": "Border#AcrylicBorder",
  "controlStyles[0].styles[0]": "Background:=<ImageBrush Stretch=\"UniformToFill\" ImageSource=\"https://raw.githubusercontent.com/kh4i-dev/wallpapers/main/start-menu.png\" />"
}
```

`ImageBrush` khong doc duoc file local, phai tro toi URL cong khai.

## Nguon anh

- `cat-bg.gif` - Pixel Art Gif Wallpaper (Keren), pixel art Mario-style
- `cat-bg.png` - pixel art mountains, resize ve luoi pixel goc 180x120
