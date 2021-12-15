
# packer-course-bootstrap

## Kickstart 

#### Générer le mot de passe de root

```bash
openssl passwd -6
```
La suite de caractére obtenu est a spécifier de la maniére suivante :
```ks
rootpw --iscrypted <password>
```

# Pré-requis d'installation 
## Note : ISO supported Rocky Linux 8

### Installez toutes les mises à jour disponibles en utilisant la commande ci-dessous :
```dnf update -y```

### Le paquet Ansible et ses dépendances ne sont pas disponibles dans les dépôts de paquets par défaut de Rocky Linux 8. Donc, pour installer Ansible via dnf, nous devons d'abord configurer le dépôt EPEL. 

### Exécutez les commandes suivantes :
```sudo dnf install -y epel-release```

### Maintenant, nous sommes tous prêts à installer ansible avec la commande dnf, exécutez :
```sudo dnf install ansible -y```

### Exécutez la commande suivante pour installer KVM :
``` `dnf install `@virtualisation host`
OR dnf install @virt virt-top libguestfs-tools virt-install bridge-utils libvirt-devel```


#### Debug

#### Augmenter le niveau de log de packer

Avant de lancer Packer définissez la variable d'environnement 'PACKER_LOG'.

```bash
export PACKER_LOG=1
```
#### Augmenter le niveau de log d'Ansible
Dans votre fichier PAcker, ajouter la configuration suivante au provisionner d'Ansible.

```hcl
    extra_arguments = [ "-vv" ]
```
