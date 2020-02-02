# Partie 1 - Introduction au Big Data
![Big Data](img/p1/big-data.jpeg)

## Les "Big Data", Pourquoi?
L'être humain, à travers l'humanité, a toujours cherché trois choses : Savoir (qu'est-ce qui s'est passé?), Comprendre (pourquoi cela s'est-il passé?) et Prédire (qu'est-ce que qui se passera?). Plusieurs cultures ont clamé l'omniscience en ayant recours à des subterfuges, tels que les oracles, l'astrologie, le tarot, ou les boules de cristal.

Cela dit, ces moyens ne sont guères satisfaisants à l'esprit méticuleux du scientifique, qui cherche toujours une explication logique et rationnelle à tout évènement, et une justification convainquante à tout comportement. Le scientifique se base sur des faits. Il veut arriver à faire de la magie grâce à la technologie.

Pour arriver à ces fins, le scientifique a besoin de données. L'intérêt de collecter des données et de les exploiter a longtemps été négligé, et a été limité au peu de données, jugées "utiles", qui semblaient suffisantes pour atteindre un objectif immédiat. Cependant, adopter le chemin évident et peu risqué n'aurait jamais permis de réaliser les miracles auxquelles on s'attendait. Il fallait trouver un autre moyen..

Le terme Big Data est apparu peu de temps après l'apparition du terme Web 2.0, qui montre la transition de l'internet d'une ère où l'ajout des données était exclusivement réservé à une élite experte, où le volume des données disponible était petit mais où les données étaient précieuses et pertinentes, vers une ère où tout un chacun était capable d'introduire des connaissances, véridiques ou pas, qui seraient sauvegardées dans une mémoire collective jusqu'à la fin des temps. Ce changement de paradigme a entrainé le besoin d'infrastructures nouvelles, qui seraient capables, non seulement de stocker ces données, mais également d'en extraire de la valeur.

Ces infrastructures auront la capacité de gérer toute la chaîne logistique des données, de la collecte vers l'affichage. Cela semble évident, me direz-vous, car les systèmes classiques sont capables de faire cela. Qui stocke mieux les données qu'une bonne vieille base de données relationnelle? Le problème est que les données dites "Big Data" sont caractérisées par des propriétés telles que, les systèmes classiques de stockage et de traitement auraient du mal à les exploiter à leur juste valeur.

## Caractéristiques des Données Massives
Le terme "données massives", ou "Big Data", ne donne à mon avis pas entièrement justice aux données de notre domaine. En effet, il représente une seule caractéristique parmis plusieurs, qui est le Volume, qui, même si elle semble être la plus importante, est loin d'être la plus critique.

En effet, les données massives sont caractérisées par les fameux *V. Il en existe plusieurs (10 jusqu'à ce jour si je ne m'abuse, mais [certains](https://www.kdnuggets.com/2017/04/42-vs-big-data-data-science.html) en citent même 42!!!), mais pourraient à mon avis être résumés en trois caractéristiques primordiales, autours de la combinaison desquelles tournent toutes les décisions prises dans ce domaine.

**Volume**
C'est évidemment le V le plus manifeste, qui caractérise le fait que les données ont un volume énorme qui peut atteindre des valeurs de l'ordre de Exa-, Zetta- ou Yottaoctet (allant jusqu'à  $2^{80}$ octets!). Mais ceci n'est pas tout. Un volume énorme, s'il reste constant, est gérable : il suffit de trouver une machine suffisamment puissante pour le gérer. Le problème avec la propriété du volume, c'est qu'il augmente de façon continue, ce qui rend sa gestion beaucoup plus ardue. Une citation bien connue, et qui se re-confirme chaque année, atteste que _"Over the last two years alone 90 percent of the data in the world was generated."_ Il est donc primordial de trouver un moyen de gérer ce volume toujours croissant des données.

**Vélocité**
Cette propriété est, à mon avis, la plus problématique des trois, car, couplée avec le volume, elle rend les système actuels obsolètes. En effet, la vélocité est, littéralement, "La vitesse avec laquelle quelque chose se déplace dans une direction particulière". Dans notre cas, la vélocité des données est la responsable directe du volume croissant des données dans le système. Elle est provoquée par une arrivée des données dans le système sous la forme d'un flux constant qui demande à être stocké et traité immédiatement, ainsi que le besoin croissant des utilisateurs d'avoir une représentation récente et fidèle de l'état des données. D'ailleurs, cette propriété a engendré une autre préoccupation des analystes des données, qui est de fournir une introspection en temps réel sur les données, les qualifiant ainsi de "Fast Data".

**Variété**
Ce qui distingue vraiment les données massives des données gérées classiquement dans des bases de données opérationnelles, c'est le support des données semi- et non structurées. En effet, les données non structurées sont des données qu'on stocke dans un format qui n'est pas défini à la création, telles que les données textuelles, images ou sons. Les données semi-structurées sont des données qui contiennent une structure, mais que cette structure n'est pas rigide, et on ne définit pas de contraintes d'écriture à l'insertion de la donnée, contrairement aux données structurées (se trouvant typiquement dans des bases de données relationnelles) qui, si elles ne respectent pas la structure définie, sont considérées fausses et ne sont pas autorisées à être enregistrées. On estime que seules 15% des données dans une entreprise sont des données structurées, contre 85% qui ne le sont pas! Dans une optique centrée sur les données, dont le but est de gagner le maximum de vision à partir des données, perdre autant de sources d'information est un vrai problème. Il est donc important que les systèmes Big Data sachent interpréter ces données et en extraire le maximum de valeur.

Toutes les décisions, choix et propriétés prises au niveau des architectures et infrastructures Big Data sont régies par ces trois caractéristiques, ce qui va complètement changer la vision "relationnelle" que tout informaticien qui se respecte a acquis tout au long de ses années d'étude et de travail.

Cela dit, ce ne sont pas les seules propriétés. D'autres V ont vu le jour, mais sans jamais avoir autant d'impact sur l'infrastructre, plutôt dans la façon de définir les processus, la gouvernance et les approches métier à adopter. Nous citons par exemple :

  - _Véracité_ : c'est la confiance que nous devons avoir en nos données. Cette propriété est inversement proportionnelle au volume et à la variété : plus nos données sont fiables, moins elles sont diversifiées et volumineuses!
  - _Valeur_ : c'est la capacité d'extraire de la valeur métier à partir des données.
  - _Variabilité_ : une extension de la variété, qui indique à quel point nos données peuvent avoir des dimensions différentes à partir des sources de données disparates.
  - _Visualisation_ : c'est la capacité de nos données à être représentées par les outils de visualisation classiques.
  - etc.

## Principes de base du Domaine des Big Data
Il est important, avant d'entamer n'importe quel travail sur les systèmes Big Data, de considérer certains principes, qui sont parfois en entière contradiction avec les principes classiques de développement d'application. Ce n'est pas si étonnant : le domaine des Big Data n'est pas censé prendre la place des domaines relationnel et décisionnel, mais plutôt les enrichir et agrémenter.

### _MOTTO 1 :_ Stocker d'abord, réfléchir ensuite
À cause de la vélocité, il est important de considérer qu'il nous sera parfois difficile, voire impossible, de nettoyer les données ou de faire un traitement quelconque dessus, avant de les stocker. Cela risque dans bien des cas de nous faire perdre des données, le cauchemar de tout scientifique des données!

Nous devons donc envisager la possibilité de définir des systèmes de stockage qui contiennent des données non nettoyées, en vrac (appelées _raw data_), pour ensuite lancer des traitements dessus.. l'horreur pour un gestionnaire de bases des données! 😱

Bien entendu, ces "bases" ne sont pas conçues pour être directement exploitées par des applications externes, mais plutôt pour conserver le plus longtemps possibles les données brutes, sans perte, qui pourraient eventuellement être réutilisées pour d'autres fins.

### _MOTTO 2 :_ Absolument TOUTES les données sont importantes!
D'où l'intérêt du _MOTTO 1_. Il nous est parfois difficile, au tout début de la conception des systèmes Big Data, de cerner toutes les possibilités offertes par ces systèmes et par les données que nous avons à notre disposition. Nous sommes donc en général tentés de supprimer les données dont nous n'avons pas besoin une fois extraite l'information immédiatement utile. Cela dit, grâce à l'accessibilité des systèmes de stockage magnétiques et leur prix de plus en plus bas, nous considérons qu'il est largement plus bénéfique de stocker des données qu'on n'utilisera peut-être jamais, plutôt que de gagner de la place et perdre un potentiel pouvoir concurrentiel.

### _MOTTO 3 :_ Ce sont les données qui pilotent le traitement
Dans un système opérationnel classique, ainsi que dans la plupart des systèmes décisionnels, ce sont les besoins métier qui prévaloient : le responsable métier commence par définir les besoins (ou les KPIs : _Key Performance Indicators_ dans le cas d'un système décisionnel), puis le responsable technique conçoit les structures de données pour répondre à ces besoins.

Par essence, un système Big Data fonctionne différemment : les données sont collectées tout d'abord à partir de toutes les sources possibles; des traitements de fouille et d'exploration de ces données sont lancés ensuite, pour extraire de la valeur à partir de ces données. L'objectif est toujours le même : chercher l'effet WOW!

D'où l'intérêt de ce MOTTO : définir le traitement à réaliser dépend des données que nous avons réussi à collecter, et par le contraire. Cela implique donc l'utilisation d'autres types de systèmes de traitement et d'algorithmes d'analyse.

### _MOTTO 4 :_ Co-localisation des données et du traitement
Un système classique à plusieurs couches, tel que le système trois tiers par exemple, se base sur le principe de séparation des données et du traitement. On trouve en général des données sur un serveur de bases de données séparé, et les traitement complexes sur un serveur d'application qui se charge de l'aggrégation et de l'affichage de ces données. Ceci est agrémenté d'un langage de requêtage déclaratif (typiquement SQL) pour réaliser des opérations de filtrage, parfois assez lourdes et complexes, au niveau de la base de données.

Cela dit, dans un contexte Big Data, le volume des données peut s'avérer assez conséquent, trop même pour envisager de le déplacer à chaque fois vers un autre système pour en extraire une vraie valeur. De plus, compter sur un langage comme SQL pour diminuer le volume ou faire de simples agrégations au niveau de la base de données pourra la rendre indisponible pendant un moment, ce qui va à l'encontre du principe de vélocité, qui exige une disponibilité à toute épreuve du système de stockage.

C'est pour cette raison que, pour réaliser les traitements voulus en un temps raisonnable et sans avoir à les déplacer sur le réseau, il est question dans les systèmes Big Data de déplacer le traitement vers les données, au lieu de déplaceer les données vers le traitement.

### _MOTTO 5 :_ La redondance, c'est bien

### _MOTTO 6 :_ Vive le Polyglottisme!

## Infrastructure Big Data : Besoins

## Théorème CAP

## Technologies et Paradigmes
### Technologies d'Ingestion de Données

### Technologies de Stockage de Données

### Technologies de Traitement de Données
