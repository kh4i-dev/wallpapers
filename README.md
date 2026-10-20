# Wallpapers

Anh pixel art cho Windows Terminal va Start menu (Windows 11).

## Files

| file | dung cho |
|---|---|
| `cat-bg.gif` | nen Windows Terminal (GIF dong, 1920x1080) |
| `start-menu.gif` | nen Start menu Windows 11 (GIF dong, 2000x1179) |

Chi con GIF: GIF la thu duy nhat ma Windows Terminal chay duoc, con PNG
phai upscale lai de khong nhhoe.

## Windows Terminal

```json
"backgroundImage": "https://raw.githubusercontent.com/kh4i-dev/wallpapers/main/cat-bg.gif",
"backgroundImageOpacity": 0.35,
"backgroundImageAlignment": "center",
"backgroundImageStretchMode": "uniformToFill"
```

## Start menu (Windows 11)

Start menu khong cho dat anh nen truc tiep. Can Windhawk + mod
*Windows 11 Start Menu Styler*:

```json
{
  "controlStyles[0].target": "Border#AcrylicBorder",
  "controlStyles[0].styles[0]": "Background:=<ImageBrush Stretch=\"UniformToFill\" ImageSource=\"https://raw.githubusercontent.com/kh4i-dev/wallpapers/main/start-menu.gif\" />",
  "controlStyles[1].target": "Border#AcrylicOverlay",
  "controlStyles[1].styles[0]": "Background:=<SolidColorBrush Color=\"#0A000000\" Opacity=\"0.65\" />"
}
```

`ImageBrush` khong doc duoc file local, phai tro toi URL cong khai.

Lop `AcrylicOverlay` den la lop scrim phia tren anh: anh giu nguyen do mo,
con scrim lam chu no len. `Opacity` cua `ImageBrush` phai la 1.0 - neu nho hon
thi app phia sau lot qua menu.

## Doi anh

```powershell
powershell.exe -NoProfile -ExecutionPolicy Bypass -File setup-startmenu.ps1 -ImageFile D:\anh.gif
```

Script tu upload len repo nay roi tro toi URL moi.
