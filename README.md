# Stickers Website

Design based on [Stylish Portfolio](https://startbootstrap.com/template-overviews/stylish-portfolio/) template.

## Games included

- Mortal Kombat
- Super Mario
- Mario Kart
- Pac Man
- Sonic

#### Custom domain

- https://www.namecheap.com/support/knowledgebase/article.aspx/9645/2208/how-do-i-link-my-domain-to-github-pages

#### Optimize images

```sh
# Converting all JPGs to progressive...
for i in products/game/**/*.jpg; do convert -strip -interlace Plane -quality 80 $i $i; done
for i in *.jpg; do convert -strip -interlace Plane -quality 80 $i $i; done
# Converting all PNGs to interlaced...
for i in products/game/**/*.png; do convert -strip -interlace Plane $i $i; done
for i in *.png; do convert -strip -interlace Plane $i $i; done
echo "Finished!"
```
