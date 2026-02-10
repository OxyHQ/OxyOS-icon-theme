# oxyos-icon-theme

Default icon themes for use with [OxyOS](https://os.oxy.so).

Based on a copy of Faenza-Darker -> Faenza-Dark -> Faenza, with greyscaled `/places` icons using:

```bash
for i in $(find . -type f -name "*.png"); do echo $i; mogrify -colorspace gray $i; done
for i in $(find . -type f -name "*.svg"); do echo $i; inkscape --batch-process --actions="org.inkscape.color.desaturate.noprefs;export-overwrite;export-do;" $i; done
```

---
Part of [OxyOS](https://os.oxy.so) | [GitHub](https://github.com/OxyHQ)
