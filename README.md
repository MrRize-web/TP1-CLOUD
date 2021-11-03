# TP1-CLOUD : Bastien Balaud



L’objectif de ce TP est de construire une image système Linux incluant le logiciel golang-myip. Ce 
dernier devra être fonctionnel et opérationnel au démarrage de la machine virtuel utilisant l’image 
disque construite. La construction de l’image système devra se faire via Packer de Hashicorp. 
Le TP est divisé en deux parties. La première est totalement accompagnée. Elle consiste en la mise 
en place d’un environnement Linux complet au sein d’une VM. Le disque de la VM est fournie 
pour plus de simplicité et est a importé dans votre outil de virtualisation favori. La VM contient un 
ISO de RockyLinux, Packer ainsi que les outils nécessaires pour la virtualisation. 
La seconde partie consiste en la prise en main de Packer et l’écriture d’un playbook (fichier 
d’instruction) Ansible pour accomplir les objectifs du TP. Cette partie est a réalisé en autonomie.




Pré-requis :
Les pré-requis du TP sont les suivants :
- Un ordinateur pouvant exécuter des machines Virtuelles X86_64 (Vmware, VirtualBox, 
KVM/Qemu (N’oubliez pas d’activer les instructions de virtualisation dans votre BIOS)
- Un client SSH (Putty, MobaXterm, etc.)
- Un client VNC pour le debugage
- Un compte Gitlab ou Github



Rendu attendu :
Le rendu se fera via le logiciel git. Les adresses des dépôts git devront être communiqués à 
mailto:bastien.balaud@gmail.com. Les dépôts git pourront être hébergés soit sur Gitlab.com ou 
bien Github.com. Si les dépôts sont privés, le compte d’utilisateur du correcteur devra être autorisé 
à accéder au dépôt. Les noms d’utilisateurs, à autoriser, sont présents en annexe. 
Le dépôt devra inclure les fichiers de configurations Packer ainsi que tout autres fichiers permettant 
d’arriver à la construction d’une image système fonctionnelle. Un fichier README est aussi 
attendu, surtout si des étapes additionnelles sont nécessaires pour parvenir à la construction de 
l’image système.
