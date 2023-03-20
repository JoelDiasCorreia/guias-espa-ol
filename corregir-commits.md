# Actualizar rama con cambios
## Autor
- Joel Dias Correia
## Instrucciones
1) obtener el codigo del commit anterior al que estoy

```bash
git log
```

2) destruir los commits y su contenidos seran llevados al arbol de trabajo

```bash
git reset --mixed "codigo del commit del paso 1"
```

3) Llevo los cambios del arcol de trabajo al staging  

```bash
git add .
```


4) Desacoplo los cambios del staging y los llevo a un stash

```bash
git stash
```

5) cambiar de rama a la rama principal 

```bash
git checkout develop
```


6) actualizar la rama principal 

```bash
git pull
```

7) crear una nueva rama 

```bash
git checkout -b "nombre de rama nueva"
```


8) para acoplar los cambios staheados anteriormente a la rama nueva basada en la principal actualizada.

```bash
 git stash apply
```

9) resolver los conflictos de merge

10) commititear los cambios ya resueltos

```bash
 git commit -m "mensaje"
```

11) pushear la rama
