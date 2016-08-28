Tarea 1

Git reset

git --soft
No toca el archivo de índice o el árbol de trabajo en absoluto (pero restablece la cabeza a <commit>, al igual que todos los modos de hacer). Esto deja a todos sus archivos modificados "Los cambios que se cometan", como git status lo pondría.

Git --mixed
Restablece el índice, pero no el árbol de trabajo (es decir, los archivos modificados se conservan pero no marcados para cometer) e informa de lo que no se ha actualizado. Esta es la acción por defecto.

Si no se especifica -N, caminos eliminadas se marcan como por intención de sumar (see git-add[1]).

git --hard
Restablece el índice y el árbol de trabajo. Cualquier cambio en los archivos rastreados en el árbol de trabajo desde comprometerse <> se descartan.

git --merge
Restablece el índice y actualiza los archivos en el directorio de trabajo que son diferentes entre <commit> y la cabeza, pero mantiene los cuales son diferentes entre el índice y el árbol de trabajo (es decir, que tiene cambios que no se han añadido). Si un archivo que es diferente entre <commit> y el índice tiene cambios unstaged, reinicio se aborta.

git --keep
Restablece las entradas de índice y actualiza los archivos en el directorio de trabajo que son diferentes entre <commit> y la cabeza. Si un archivo que es diferente entre <commit> y HEAD tiene cambios locales, reinicio se aborta.


