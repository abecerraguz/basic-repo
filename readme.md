#VER EL PASADO

##Muestra todos los commit

```git log / git log -1 (Muestra solo un commit)
```
```Agregando la opción -p, le dice a Git que muestre el diff de cada versión creada
git -p
```

```Para ver cuanto ha cambiado desde el commit 18f822eb1044761f59aebaf7739261042ae10392, ejecutamos:
git diff --stat 18f822eb1044761f59aebaf7739261042ae10392
```

#REVIRTIENDO CAMBIOS
Aquí tenemos 2 formas de volver atrás a un commit anterior: revertir (revert) y reiniciar (reset). Vamos a comenzar con revert y es recomendado que intentes usar revert por sobre reset siempre que sea posible.

La forma más simple de revertir un commit existente es con el comando git revert. El "revierte" un commit creando un nuevo commit en tu repositorio que reversa todos los cambios realizados por el commit original.

```git revert -n 540ecb7 
```

#REINICIAR RESET

¡¡¡Advertencia!!! Cuando hacemos reinicio de los cambios usando este comando, los cambios que revertimos se PIERDEN PARA SIEMPRE

```se puede usar 7 caracteres del has
git reset 6c77676 --hard
```

```Se puede hacer el reset de un archivo
git reset <commit hash> <filename> --hard
```