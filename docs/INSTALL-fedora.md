# Installer et lancer my_navy sur Fedora

Testé sur Fedora 39 (GCC 13). Aucune dépendance en dehors du compilateur.

```bash
sudo dnf install gcc make
git clone git@github.com:FuniclemDev/navy-source.git
cd navy-source
make
```

Ouvrez deux terminaux dans le dossier :

```bash
# Terminal 1
./my_navy pos1            # affiche « my_pid: 12345 »

# Terminal 2
./my_navy 12345 pos2      # remplacez par le PID affiché
```

Tapez ensuite une case (`A1` … `H8`) quand le jeu affiche `attack:`.
`./my_navy -h` affiche l'aide. Un fichier de flotte invalide arrête le programme avec le code 84.
