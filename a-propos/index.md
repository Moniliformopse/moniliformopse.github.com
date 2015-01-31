---
layout: page
title: A propos
excerpt: "So Simple is a responsive Jekyll theme for your words and images."
modified: 2014-06-23 10:09
image:
  feature: moniliformopse_equisetum.jpg
  credit: Shin5963
  creditlink: https://www.flickr.com/photos/87384485@N08/13683763013/
---

# Moniliformopse.github.io



Blog personnel de Vincent Thizeau, agrégé de l'Université, professeur des Sciences de la vie et de la Terre (SVT), webmestre du site internet du [lycée Louis Bascan](http://www.lyc-bascan-rambouillet.ac-versailles.fr/) - Rambouillet (78)



Le titre du blog fait référence à un groupe de végétaux de la lignée verte dont voici quelques représentants : les prêles des champs (*Equisetum arvense*) de la famille des Sphénophytes ; le polypode commun (*Polypodium vulgare*), l'osmonde royale (*Osmunda regalis*) et la fougère aigle (*Pteridium aquilinum*) tous les trois de la famille des Filicophytes.
{: .notice}



Adresse du blog : [http://moniliformopse.github.io](http://moniliformopse.github.io/)



Propulsé par Jekyll avec *So Simple Theme* traduit en français.

<figure>
	<img src="http://bit.ly/1md8csQ">
	<figcaption>écran du blog Moniliformopse</figcaption>
</figure>

---



## Technologies utilisées



Ce blog fonctionne avec [Jekyll](http://jekyllrb.com/) un générateur de pages HTML statiques, en absence de base de données. Son contenu est rédigé en [Markdown](http://daringfireball.net/projects/markdown/).



Le support de publication, le code spécifique de ce blog et son identité graphique sont redevables à [Michael Rose](http://mademistakes.com/) auteur du thème [So Simple](http://mademistakes.com/articles/so-simple-jekyll-theme/) pour Jekyll.



L'identité graphique de ce site utilise les outils suivants :


- LESS ->  [http://lesscss.org/](http://lesscss.org/)

- des variables [LIQUID](http://docs.shopify.com/themes/liquid-basics), pour la création des pages.



[Retrouvez toutes les caractéristiques du thème sur GitHub](https://github.com/mmistakes/so-simple-theme/).



L'ensemble est hébergé par [GiHub](https://github.com/) selon les modalités de [GitHubPages](https://pages.github.com/).


Le blog propulsé par Jekyll n'utilise pas de langage serveur dynamique : cela signifie qu'il n'y a pas de traitement,  ni de validation et ni d'analyse de données. Il a donc fallu passer par le service annexe offert par [Disqus](https://disqus.com/) (gratuit) pour avoir un formulaire de commentaires.


---


## Conception et mise en oeuvre



Cest grâce à tous ces outils (librement mis à disposition) que la personnalisation de l'habillage graphique de ce blog et sa traduction française ont été développées pour le plaisir par Moniliformopse -> [http://moniliformopse.tiddlyspace.com/](http://moniliformopse.tiddlyspace.com/)



---

## Installation



**Ruby**



Jekyll est développé en [Ruby](https://www.ruby-lang.org/fr/), il faut donc vous assurer que ce dernier est présent sur votre machine.



Pour MacOS X, vous avez une version de ruby (1.8.7), ce n'est pas la dernière mais elle est suffisante pour nos besoins. Si néanmoins vous souhaitez avoir la dernière version, le mieux est de faire la mise à jour avec [Homebrew](http://brew.sh/index_fr.html).


{% highlight bash %}
$ ruby -e "$(curl -fsSL https://raw.github.com/mxcl/homebrew/go)"
{% endhighlight %}

{% highlight bash %}
$ brew install ruby
{% endhighlight %}



Pour Windows, le plus simple est d'utiliser l'installateur. Vous pouvez le télécharger à cette adresse -> [http://rubyinstaller.org/downloads/](http://rubyinstaller.org/downloads/)



**Jekyll**



Une fois Ruby installé, il vous suffit de lancer la commande suivante dans un terminal pour installer Jekyll :


{% highlight bash %}
$ gem install jekyll
{% endhighlight %}



Pour installer le thème *So Simple* pour Jekyll, lire la documentation de son auteur -> [https://github.com/mmistakes/so-simple-theme/](https://github.com/mmistakes/so-simple-theme/)

---



## Structure complète du blog



{% highlight bash %}
so-simple-theme/
├── _includes/
|    ├── browser-upgrade.html   # prompt to install a modern browser for < IE9
|    ├── disqus_comments.html   # Disqus comments script
|    ├── footer.html            # site footer
|    ├── head.html              # site head
|    ├── navigation.html        # site top navigation
|    ├── open-graph.html        # Twitter Cards and Open Graph meta data
|    └── scripts.html           # site scripts
|    └── site-search.html       # site search overlay
├── _layouts/
|    ├── page.html               # single column page layout
|    └── post.html               # main content with sidebar for author/post details
├── _posts/                      # MarkDown formatted posts
├── _sass/                       # Sass stylesheets
├── _templates/                  # used by Octopress to define YAML variables for new posts/pages
├── about/                       # sample about page
├── articles/                    # sample articles category page
├── assets/
|    ├── css/                    # compiled stylesheets
|    ├── fonts/                  # webfonts
|    └── js/
|        ├── _main.js            # main JavaScript file, plugin settings, etc
|        ├── plugins/            # scripts and jQuery plugins to combine with _main.js
|        ├── scripts.min.js      # concatenated and minified _main.js + plugin scripts
|        └── vendor/             # vendor scripts to leave alone and load as is
├── blog/                        # sample blog category page
├── images/                      # images for posts and pages
├── 404.md                       # 404 page
├── feed.xml                     # Atom feed template
├── index.md                     # sample homepage. lists 5 latest posts 
└── theme-setup/                 # theme setup page. safe to remove
{% endhighlight %}


---


## Configuration



Consulter les informations contenues dans la page  [Theme Setup](http://moniliformopse.github.io/theme-setup/)

---



## Intégration dans un article



- [La coloration syntaxique](http://moniliformopse.github.io/articles/code-highlighting-post/) (*Syntax Highlighting Post*)



- [Un simple lien](http://moniliformopse.github.io/articles/sample-link-post/) (*Sample Link Post*)



- [Une vidéo](http://moniliformopse.github.io/articles/video-post/) (*A Post with a Video*)



- [Une image et un long texte](http://moniliformopse.github.io/articles/readability-feature-post/) (*Post with Large Feature Image and Text*) 



- [Plusieurs images de tailles variables](http://moniliformopse.github.io/articles/sample-post-images/) (*A Post with Images*)



- [La lisibilité d'un texte](http://moniliformopse.github.io/articles/readability-post/) (*Testing Readability with a Bunch of Text*) 



- [Un article test](http://moniliformopse.github.io/articles/sample-post/) (*Sample Post*) 

---



## Compatibilité



- Jekyll (dernière version testée : 2.5.3)

- Bureau : IE 9+ (Accessible IE 7&8), Firefox, Chrome, Safari.

- Mobile : à peu près tous les navigateurs mobiles modernes.


---


## Performances



Mesurées sur [PageSpeed Insight](https://developers.google.com/speed/pagespeed/insights/) :



**pour mobile et tablette**


- vitesse : 61/100

- expérience utilisateur : 99/100



**pour ordinateur portable et de bureau**


- environ : 81/100