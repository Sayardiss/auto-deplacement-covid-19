# Générateur automatique de certificat de déplacement

## C'est pour voler des données ?

Non, savoir que tu sors, ça intéresse que ton mari ou ta mère. Je m'en cogne, et le gouvernement affirme s'en foutre aussi.  
Si tu ne me crois pas, alors n'utilise pas. Si tu veux savoir comment ça fonctionne, pour que je ne garde rien :
- tout est fait côté client (ton portable, ton PC...) en JavaScript
- à aucun moment je ne stocke les informations indiquées
- libre à toi de croire le gouvernement. Je peux te donner ce lien, si tu veux plus d'info : https://media.interieur.gouv.fr/deplacement-covid-19/confidentialite.html.

J'ai moi-même analysé le comportement du site d'origine, et je confirme que rien n'est envoyé.

## Qu'est ce qui prouve que c'est pas un malware ?

C'est juste un site web, pas besoin de t'affoler. Rien à installer sur ton téléphone, je ne vais pas allumer ta caméra car j'ai pas envie de te voir.  
Ici, tu vas trouver le code source.  
Je me suis basé sur le code source fourni par le gouvernement, et j'y ai ajouté une trentaine de lignes. Tu peux les voir à ton aise, ou demander à quelqu'un de confiance de regarder, si tu ne t'y connais pas.

## Comment l'utiliser ?

La première fois, c'est pas très facile, mais une fois que c'est fait, il n'y a plus rien à faire !

Copie-colle ce lien dans ton navigateur :

https://sayardiss.github.io/?nom=DUPONT&prenom=Hervé&date_n=28/01/1990&lieu_n=Bordeaux&adresse=1%20rue%20des%20cerisiers&cp=75001&ville=Paris&raison=faj

- nom = ton nom
- prenom = ton Prénom
- date_n = ta date de naissance, au format 31/01/2000
- lieu_n = ton lieu de naissance
- adresse = ton adresse. ici, c'est 1 rue des cerisiers, ne t'inquiète pas les espaces sont remplacés par "%20" c'est normal
- cp = ton code postal
- ville = tu vas deviner
- raison = alors là on attaque le plus compliqué. Tu peux mettre plusieurs lettres, sachant que :
  - f famille/personne vulnérable
  - c courses de première nécessité
  - a activité sportive
  - t travail
  - j judiciaire
  - m missions TIG
  - s santé

Dans l'exemple, **raison** vaut *faj* donc famille, activité sportive et judiciaire. Si rien n'est mis, ça sera courses !

## J'ai regardé ton code source, c'est mal codé !!

OK. Je suis pas dev, je te laisse me proposer un truc plus propre :)


## Crédits

Ce projet a été réalisé à partir d'un fork du dépôt [deplacement-covid-19](https://github.com/LAB-MI/deplacement-covid-19).
