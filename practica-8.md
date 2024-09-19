# Practica 8
## Repaso de lo visto en clase sobre Git y Git hub

### a. ¿Cómo se inicializa un repositorio en Git?

Se usa el codigo:
```bash
git init
```

### b. ¿Cómo creas un repositorio en GitHub?

Se ve un icono de un libro con una etiqueta que dice "new", al darle click es ponerle un nombre que sea amigable con la configuracion por ejemplo (practica-8-3dev) todo minusculas, (-) espacios, por ultimo elegir si privado o publuco y ya darle click a "create repository".

### c. ¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?

Despues de ya tener un repositorio hecho, en la terminal de visual studio se debe de poner:
```bash
git remote add origin https://github.com/tu-usuario/nombre-repositorio.git
```

### d. ¿Cuál es el flujo básico de trabajo en Git y GitHub?

Directorio:
```bash
git add . / git add archivo/directorio
```
Staged/Staging:
```bash
git commit / git commit -m "Mensaje"
```
Commited:
```bash
git push -u origin master (1ra vez) / git push
```
Remote/Remoto:
```bash
git pull
```
Directorio: (volvemos a empezar)

### e. ¿Para qué sirve el archivo .gitignore?

Ayuda a especificar qué archivos o carpetas no deben ser incluidos en el repositorio, estos incluso se vuelven invisibles.

### f. ¿Cuál es el propósito de una rama?

Permite trabajar en diferentes versiones del mismo proyecto sin afectar a la rama principal.

### g. ¿Qué es una fusión?

Es un proceso para combinar los cambios hechos de una rama a otra
Estando en la rama en la que se quedara la fusion hacer el comando:
```bash
git merge rama-secundaria
```

### h. Explica los diferentes tipos de fusión que existen.

Hay 2:

**Fast-Forward**: Se juntan directo no hay conflictos al juntar las ramas.

**Manual Merge**: Se hace de forma manual debido a que se sobrepone el contenido y esto genera problemas.

### i. ¿Cómo puedes ver el historial de tu repositorio?

Se usan 2 comandos:

Muestra completo el historial
```bash
git log
```
Muestra solo una linea por cada cambio realizado (Historial Resumido)
```bash
git log --oneline
```

### j. ¿Cuál es el propósito de una etiqueta?

Normalmente se usa para señalar versiones en las que se va progresando el repositorio, codigo, documento,etc...