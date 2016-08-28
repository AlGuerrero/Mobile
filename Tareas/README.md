Tarea 1

Git resett

git soft
--suave
No toca el archivo de índice o el árbol de trabajo en absoluto (pero restablece la cabeza a <comprometen>, al igual que todos los modos de hacer). Esto deja a todos sus archivos modificados "Los cambios que se cometan", como git status lo pondría.

--mezclado
Restablece el índice, pero no el árbol de trabajo (es decir, los archivos modificados se conservan pero no marcados para cometer) e informa de lo que no se ha actualizado. Esta es la acción por defecto.

Si no se especifica -N, caminos eliminadas se marcan como por intención de sumar (ver git-add [1]).

