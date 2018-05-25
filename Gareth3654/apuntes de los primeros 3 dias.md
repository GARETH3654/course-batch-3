notas de primera y segunda clase 

Reglas de Oro
 1.-git pull upstream master
 2.- trabajar en local
 3.-git add . o file/directory
 4.-git commit -m ""
 5.-git pull upstream master *solo si no hay merge
 6.-
    6.1 git push origin
    6.2 pull request
 7 resolver conflictos manuales (bugs)

Sistemas de tageo 
x.y.z
x= cambios publicos - son cambios que se modifican y se cashean con el original
y=new featuring - son cambios pero sin afectar el diseño principal
z=solucion de errores - son cambios por dentro del sistema, como mejorar el rendimiento y/o optimizar la pagina 

CHANGEDLOG.md
 es importante poner la actualizacion (5.0.3) y poner las caracteristicas de las    actualizaciones
 
 dia 2
  Github 
 Github es una plataforma virtual la cual nos ayuda a guardar nuestro codigo creado desde un local y este crea un repositorio y ahí es donde se guarda nuestro codigo
 algunos comandos para git son estos :
`git remote -v` => Indica los remotes sincronizados en local
`git remote add <remote_alias> <ssh/https url>` => Agrega un remote a nuestro local
`git pull <remote> <branch>`
`git remote remove <remote_alias>`
`git branch <branch_name>` => Crea una rama
`git checkout <branch_name>` => Cambiar a la rama branch_name
`git checkout -b <branch_name>` => Crea una rama y nos cambia a ella
`git branch -d <branch_name>` => Borra la rama (No debemos estar en ella)
`git branch -D <branch_name>` => Borra la rama aunque tenga commits o cambios pendientes.
`git merge <branch_name>` fusiona las branches (la que estamos posicionados) con la branch_name
`ssh-keygen` => para generar ssh keys
`pbcopy < ~/.ssh/id_rsa.pub` => Copia la llave pública

dia 3 del curso
ECMAscrip6
con anterioridad se usaba:
    var boo= '';
pero ahora existen dos nuevos tipos de variables que son: (estan son las que usaremos en este curso)
    const boo='';
    let boo= '';
    
antes para trabajar funciones tenias que llamar una funcion
    function hello() {
        //@todo
    };

ECMascrip (estandar) 6
javascript (lenguaje) 2015


ahora una funcion funcionaria con 
    const hello= ( name='') =>{
        //@todo
    }
 con ECMAscrip6 podemos inicializar un parametro en la declaracion de la funcion

// es6
if
if else

switch
    vamos a usarlo envez de usar ifelse si hay mas de dos condicionales  
       switch(option){
        case: 1
        break;
        case: 2
        break;
        case: 3
        break;
        case: 4
        break;
        default:
        }
condition ? true : false; 

ciclos
for(var i = 0; i < array.length; i++){
    array[i]
}
lo nuevo de los ciclos:
    for(const index in array){
     console.log(index); //0,1,2
    }
el sig. es 
    for(const iterable of array){
    console.log(iterable); // 1,2,3
    }    
for of- lista de arreglos
for in - optimizado para la familia de los objetos

for in .Los for in son propiedades enumerables(se pueden contabilizar los indices y/o propiedades de un array), es normal usar de for-in es usado para esculpir las propiedades de un objeto
 
 for each pertenece exclusivamente a la familia real de los array el metodo for each se introdujo en el linaje de de la herencia del ArrayObject
for of crea un ciclo interativo con los arreglos iterables

array.map - map usa una funcion anonima como parametro para saber que es lo que vas a hacer.

 ejemplo:
const newArray = users.map((user) =>{
    return{
        fullName: `${user.lastName}, ${user.name}`(esto es nuevo en ECMAstrict 6 "string templates")
        };
});

const user =[{
    name: 'alfonso'
    lasteName 'Ríos'
}];





