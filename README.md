# trunk-based-branching-lab
Trunk based Development branching lab 


A continuacion se enlistan los pasos a seguir para generar un repositorio con la estrategia de branching trunk based:

0. Creacion de repositorio
![1 -new-repository](https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/5d417045-465c-473f-b746-df7985657acf)


1. Clonar el repositorio: `git clone git@github.com:jc-esquivelojeda/trunk-based-branching-lab.git` 
<img width="757" alt="3 -git-clone" src="https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/28f9ed81-9183-495e-a972-62d8d8853ed9">


2. Acceder al directorio donde se clono el proyecto base: `cd trunk-based-branching-lab`
3. Verificar el estatus del proyecto: `git status`
4. Generar una rama para el feature a crear: `git checkout -b feature/improved-readme`
<img width="757" alt="4 -create-new-feature" src="https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/d853cfaa-d1cd-414c-addf-8a0a41be4708">

5. programar el "feature" `nano README.md`
6. Agregar los cambios para ser guardados `git add .`
7. Verificar que no queden cambios pendientes: `git status`
8. Guardar los cambios: `git commit -m "[feature] added descriptive message to readme.md"`
9. Guardar los cambios en remoto: `git push --set-upstream origin feature/improved-readme`
<img width="761" alt="6 -Pushed-changes-to-remote" src="https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/65debe0a-1430-4fe5-af38-89437d0aa8ce">

10. Cambiar a la rama principal `git checkout main`
11. Verificar que se encuentra en la rama correcta: `git branch`
12. Mezclar los cambios en la rama principal: `git merge feature/improved-readme`
<img width="643" alt="7-merge-changes-into-main" src="https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/0ec6b42d-eb4c-46f0-a7a9-6b9df6e4ef28">

13. Eliminar localmente la rama: `git branch -d feature/improved-readme`
14. Eliminar la rama remota del feature: `git push origin --delete feature/improved-readme`
<img width="727" alt="10 -deleted-merged-branch" src="https://github.com/jc-esquivelojeda/trunk-based-branching-lab/assets/123103329/fb8f33a9-58a5-4a02-9c3e-b785627e4035">


