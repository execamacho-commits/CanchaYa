# Cómo mostrar el repositorio de CanchaYa

1. En Windows, descargá y extraé todo el ZIP. La carpeta extraída contiene este archivo y la carpeta oculta .git. Esa carpeta contiene el historial.
2. Abrí Git Bash en la carpeta extraída. Si no tenés Git instalado, instalá Git for Windows antes de continuar.
3. Ejecutá estos comandos, de a uno.

```bash
git status
git branch -a
git log --graph --oneline --all --decorate
git show --stat v1.0.0-docs
```

El primer comando muestra la rama actual y si hay cambios pendientes. El segundo lista las ramas. El tercero dibuja el historial. El cuarto muestra la etiqueta de la entrega documental y el resumen del commit al que apunta.

Para explicarlo en clase: «En main dejamos la versión de entrega. En develop integramos los avances. Se crearon ramas separadas para el alcance, el modelo de datos y la validación prevista. El historial registra la preparación de la documentación con asistencia de Codex».

## Cómo obtener un enlace de entrega

Creá un repositorio vacío en GitHub o GitLab, sin README inicial. Copiá su URL HTTPS y, desde la misma carpeta, ejecutá lo siguiente reemplazando URL_DEL_REPOSITORIO por esa dirección.

```bash
git remote add origin URL_DEL_REPOSITORIO
git push -u origin main
git push origin --all
git push origin --tags
```

Iniciá sesión si la herramienta lo pide y verificá en el sitio que aparezcan las ramas y el historial. Compartí con los profesores la URL del repositorio. Si es privado, otorgales acceso por el mecanismo indicado por la cátedra.
