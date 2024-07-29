> [!INFO]
> Ici se trouvent mes remarques pour le projet Devloweb



## Nom de domaine
Il faut absolument racheter ce nom de domaine ARGH

## Création d'une template
> Ceci est un petit guide pour vous guider dans la création d'une template compatible **Devloweb**

Tout d'abord on commence avec une structure JSON
```json
{  
  "header": {  
    "title": "Devlowave",  
    "navlink": [  
    ]  },  "hero": {  
    "headline": "",  
    "subheadline": "",  
    "cta": ""  
  },  
  "about": {  
    "title": "",  
    "description": ""  
  },
  "footer": {  
    "copyright": "",  
    "social_links": [  
      "",  
      "",  
      ""  
    ]  
  }}
```

Chaque **section** porte un nom qui sera représenté ainsi dans le fichier **html** :
```html
<section class="hero">  
    <div class="container">  
        <input type="text" id="hero-headline" name="hero-headline" class="text-input" value="Making a Difference, One Step at a Time">  
        <input type="text" id="hero-subheadline" name="hero-subheadline" class="text-input" value="Join us in our mission to create a better world for everyone.">  
        <input type="text" class="btn text-input" id="hero-cta" name="hero-cta" value="Donate Now">  
    </div>  
</section>
```
-> Les *id* permettent au générateur de savoir à quel endroit stocker les éléments du site.

> [!IMPORTANT]
> Les éléments sont stockés de cette manière :
> - \[section]\[item]\[rank]
> - section : *str*
> - item : *str*
> - rank : *int*
> Donc par exemple, l'id "**header-navlink-1**" sera stocké ainsi :
> ```json
> {
> "hero": {
> 	navlink: ["ici"]
> 	}
> }

