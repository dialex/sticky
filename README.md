# Stickers Website

Design based on [Stylish Portfolio](https://startbootstrap.com/template-overviews/stylish-portfolio/) template.

## Games included

- ~~Kingdom Hearts~~
- Mortal Kombat
- ~~Angry Birds~~
- ~~Neko Atsume~~

- Super Mario
- Mario Kart
- Pac Man
- Sonic

#### Optimize images

```sh
echo "Converting all JPGs to progressive..."
for i in products/game/**/*.jpg; do convert -strip -interlace Plane -quality 80 $i $i; done
echo "Converting all PNGs to interlaced..."
for i in products/game/**/*.png; do convert -strip -interlace Plane $i $i; done
echo "Finished!"
```
