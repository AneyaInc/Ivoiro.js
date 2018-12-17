# Ivoiro.js

### Par Gabeta Soro, [Medium Blog](https://medium.com/@gabeta.soro) 2018

En pensant je me suis pourquoi télécharger 50Ko voir même plus et souvent dépendre de Jquery pour formatter ses montants en CFA. 
Le but c'est de se passer des Kilo JS pour faire des choses simple comme formatter un montant en CFA, Formatter un numéro de téléphone exemple : (+225) 00 00 00 00 / 
(+225) 000 00 000 ... Connaitre le réseaux d'un numéro de téléphone.

## Getting Started

1. Télécharger [Dernière version](https://github.com/EnighmaLab/Ivoiro.js/releases/latest)
2. Inclure le JS ivoiro

```html
  <script src="chemin/vers/ivoiro.js"></script>
```

3. Ajout et initialisation du plugin

```html
<span class="cfa-format">100000</span><br>

<script src="chemin/vers/ivoiro.js"></script>
<script type="text/javascript">
  var ivoiro = new Ivoiro({
    className: 'cfa-format'
  });

  ivoiro.formatToCfa(' ', true);
</script>
```

- Le premier paramètre de la fonction formatToCfa est le séparateur 
  exemple : 1000 si vous mettez le séparateur à . alors vous aurez 1.000
  idem pour 1000000 vous aurez 1.000.000

- Le sécond paramètre design si le montant doit être préfixé par default 
  Exemple: si le paramétre est à true et séparteur à . pour 1000 on aura 
  1.000 CFA

## Contribuer

Faites un fork du projet. Ajouter vos modifications et faites moi un
pull request.
