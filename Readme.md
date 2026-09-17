# TP1 - Installation Linux sur une VM - V0.4

## Groupe 

1. Yazan (YAD) 		- Noé (NAM) 
2. Siméon (SAR) 	- Gaëtan (GFR)
3. Tristan (TCK) 	- Nicolas (NTN)
4. Matéo (MCN) 		- Thomas (TBT)
5. Noah (NRN) 		- Guillaume (GFE)
6. Benjamin (BSC) 	- Valentin (VBC)
7. Gabriel (GOM) 	- Nikola (NDC)

## But 

Cette manipulation a pour but d'installer une distribution linux [Sparky Linux](https://sparkylinux.org/) dans une machine virtuelle VMware 
Workstation Player, à l’aide d’une image disque (ISO).

## Materiels à disposition 

- VMware Workstation Player - V17
- Image disque (ISO) : sparkylinux-6.4-x86_64-minimalcli.iso

## Création d’une machine virtuelle 

**A.** Lancez VMware Workstation Player (logiciel)  

**B.** Sélectionnez **Create a New Virtual Machine** 

**C-A.** Placez le fichier `.iso` dans une repertoire connu : 

`C:\VosInitiales\VM\ISO`

**C-B.** Indiquez le chemin d’accès de l’image iso comme indiqué sous l’image ci-dessous :

![install image disk](/Images/Install_ISO.jpg) 

**D-A.** Choisissez un nom d'OS : `Linux - Debian 11.x` 

![OS name choice](Images/OS_Choice.jpg) 

**D-B.** Nommez la machine virtuelle : `SparkyLinux-VosInitiales` 

**E.** Creez un disque virtuel -> capcité : **20GB** 

> Remarque 1 : Cocher **store virtual disk a single file**

![Virtual disk](/Images/VirtualDisk.jpg) 

> Remarque 2 : Ci-dessous, la configuration de la VM 

![Virtual disk](/Images/VM_Config.jpg) 

**F.** Lancez la machine virtuelle : **Play virtual machine** 

## Lancement de l'image ISO (Linux - Live_CD) 

**G.** Lancement du live CD : 

![install image disk](/Images/live_CD.jpg) 


Shell Linux : 

[Placer votre capture d'écran]() 

> **ATTENTION** : par défaut, le clavier est configuré est **Clavier Americain**

Q1. disposition du clavier américain ?

> votre réponse ?!

Q2. disposition du clavier suisse-romand ?

> votre réponse ?!

Q3. disposition du le clavier français ? 

> votre réponse ?!

**H.** Déplacez-vous à la **racine du système** en utilisant la commande suivante : `cd` 

Q4. vore commande ?!

**I.** Affichez le contenu de la racine avec la commande : `ls –l`	

![Placer votre capture d'écran]() 

Q5. Que signifie l'option `-l` avec la commande `ls` 

> votre réponse ?!

Q6. Décrypter la ligne où se trouve le répertoire **home**    

[Placer votre capture d'écran]()

> votre réponse ?!

**J.** Créez un répertoire de travail nommé « EMSY_VosInitiales» 

Q7. dans quel dossier racine allez-vous le placer (justifiez votre réponse) 

> votre réponse ?! 

Q8. Quelle commande allez-vous utiliser pour faire ceci ?  

> votre commande ?! 

**K.** Dans ce répertoire, créez un fichier texte que vous nommerez `TESTSLO_XXX_XXX` et éditez celui en écrivant un texte, exemple : "TP linux by XXX et XXX".
	   Utiliser la commande `vi`

> votre commande ?! 

Q9. Pouvez-vous éditez un fichier uniquement avec la commande `vi` 

> votre réponse ?!

Q10. Si vous éteignez la machine virtuelle et que vous la rallumez, est-ce que le répertoire créé ci-dessus existe toujours (justifiez votre réponse) ? 

> votre réponse ?!

**L.** Tapez la commande `ls -l /dev/sda` 

![Placer votre capture d'écran]() 

Q11. Que signifie **sda** ? 

> votre réponse ?!

Q12. Quelle différence y a-t-il entre le répertoire de la question Q6 et celui du point L (justifiez votre réponse) ?

> votre réponse ?!

## Installation de SparkyLinux sur la VM

**M.** Installez SparkyLinux

![Placer vos captures d'écrans de l'installation]()

Q13. Quelle est la taille de disque minimum recommandée pour installer la distribution Sparky en mode cli 

> votre réponse ?!

Q14. A quoi sert la partition swap ? Est-ce que ce principe existe-t-il sur les OS Microsoft Windows ? 

> votre réponse ?!

Q15. Quel format pourriez-vous utiliser pour la 3ème partition afin qu’elle soit également accessible depuis un OS Microsoft ? 

> votre réponse ?!

Q16. Durant l’installation, on vous demande deux noms d’utilisateur. A quoi correspondent-ils ? 

> votre réponse ?!

**N.** Une fois l’installation de Linux terminée, prenez une capture d’écran du démarrage de votre système (GRUB)

![Placer votre capture d'écran]() 

**O.** Trouvez la ou les lignes de commande permettant de changer le clavier et procédez à la configuiration 

> votre commande ?! 

![Placer votre capture d'écran]() 

**P.** Tapez la commande : `nano -version`

![Placer votre capture d'écran]() 

Q17. A quoi sert `nano` ? 

> votre réponse ?!

**Q.** Testez si l’application `git` est installée sur votre distribution, si ce n’est pas le cas installez un client git. 

Q18. Comment savoir si `git` est déjà installé ? 

> votre réponse ?!

> votre commande ?! 

Q19. Si le client `git` n'est pas installé, quelle(s) commande(s) utilisez-vous pour l’installer ? 

> votre commande ?! 

Q20. Que veut dire `apt` ? 

> votre réponse ?!

Q21. Est-ce que cette commande (`apt`) peut être utilisée sur toutes les distributions Linux (justifiez votre réponse)? 

> votre réponse ?!

**R.** Créez un sous-répertoire « EMSY_TP1_XXX-YYY » dans le répertoire de votre utilisateur. 
       
**Attention** : Ici on veut que l’utilisateur (vous) ait les droits de lecture, d’écriture et d’exécution.

> votre commande ?! 

Q22. Quel est le répertoire utilisateur ?  

> votre réponse ?!

Q23. Quelles sont les commandes pour changer les droits d'utilisateurs (lecture - écriture - execution) ?  

> votre commande ?! 

**S.** Dans ce répertoire, tapez la commande : `git clone https://github.com/votreDepot/EMSY_TP1_Source`

***Remarque*** : Il faut au préalable que vous ayez mis en place à cette adresse un fork du dépôt fourni lors de ce TP.

Q24. Qu’observez-vous dans ce répertoire ?

![Placer votre capture d'écran]()

**T.** Editez le fichier source `.c` avec l’éditeur de texte « nano ». -> Réalisez un petit programme en C (par exemple de type « Hello world »).

![Placer votre capture d'écran]()

**U.**	Vérifiez si le compilateur `gcc` est bien installé. Notez la version du logiciel

> votre réponse ?!

![Placer votre capture d'écran]()

**U-A.** Tapez les commandes suivantes :
```Shell 
gcc -Wall -o fichier.o -c fichier.c 
gcc -o fichier fichier.o 
```
Remarque : « fichier » est à remplacer par le nom de votre choix

![Placer votre capture d'écran]()

Q25. Quels sont les fichiers qui ont été générés 

> votre réponse ?!

![Placer votre capture d'écran]()

**V.** Entrez la commande suivante : `./fichier`

![Placer votre capture d'écran]()

Q26. Que se passe-t-il ?

> votre réponse ?!



...A compléter...

## Tips 

> Tip 1 : sortir de la VM -> appuyer simultanément sur `Ctrl` et `Alt` 

> Tip 2 :  
> Pour arrêter un Linux proprement : 	`shutdown`  
> Pour forcer l’arrêt d’un système :	`halt` ou `poweroff`  
> Seul un administrateur peut exécuter ces commandes !

> Tip 3 : [commande vi avec ses options](https://www.linuxtricks.fr/wiki/guide-de-sur-vi-utilisation-de-vi)

> Tip 4 : [éditer un fichier type markdown (.md)](https://ashki23.github.io/markdown-latex.html)

