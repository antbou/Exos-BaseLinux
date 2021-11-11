# Some bash command

```sh
# Tapez **man man** et retrouvez l'option permettant d'afficher la description courte des pages du manuel correspondant.
man -f man

# Demander confirmation avant toute destruction de fichier
rm -i

# Affichez la liste des fichiers du répertoire /var/log triée par date de modification pour voir quel est le fichier de logs du système le plus récent.
 ls -lh --sort=time /var/log

 # Avec la commande *sort*, triez ce fichier par *ordre alphabétique inverse*
 sort -r usrLocal.txt > inverse.txt

# Afin d'éviter de devoir répondre par *y* à chaque suppression de fichier, utilisez la combinaison adéquate permettant d'envoyer cette réponse par la commande *yes*
 yes | rm -i ./bonjour
```

|  Droits       |  Octal |  Symbolique          |
| ------------- | ------ | -------------------- |
| `rw- -w- ---` | 620    | chmod u=rw,g=w,o=-   |
|               |
| `rwx -wx --x` | 731    | chmod u=rwx,g=wx,o=x |
|               |
| `r-x -w- --x` | 521    | chmod u=rx,g=w,o=x   |
|               |
| `--x --x r--` | 114    | chmod u=x,g=x,o=r    |

## Other basic command :

```sh
# create file: > file.txt OR touch file.txt
count file: ls | wc -l

remove directoy recursive: rm -r directory

#find all files containing specific text:

grep -rnw '/path/to/somewhere/' -e 'pattern'

# direcotry size:
du -h

# file size:
ls -lh files.zip

# find file all:
find -name "*44"

# find folder not recursive:
find -maxdepth 1 -type d -iname "*1"

# display actual location:
pwd

# display hash :
md5sum

# zip / unzip directoy :
zip -r tes1t.zip tes1t / unzip tes1t.zip

# tar / untar :
 tes1t.zip tar -zcvf test.tar.gz test/ OR tar -zcvf test.tar.gz test/

# find word in file :
grep -n asdsadsad blabla.txt

rsync : rsync -av old/folder/ new/folder

```
