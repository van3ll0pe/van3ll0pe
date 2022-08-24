# BIENVENUE

Je suis **van3ll0pe**

J'adore le **C**, **python** et les **réseaux informatiques**.

---
Je sais que les pointeurs peuvent poser problèmes dans l'apprentissage du C alors je voulais vous faire un *RECAP*

>`&` signifie l'adresse mémoire

>`*` signifie la valeur à l'adresse mémoire

donc si je crée un pointeur en faisant : `ptr = &a`
le pointeur stocke l'adresse mémoire de a.

Si je fais `*ptr` j'obtiens la valeur de a, donc je suis capable de modifier la valeur d'une variable en passant par un pointeur en faisant : `*ptr = new value`

Si je veux faire la même chose avec un pointeur alors je dois utiliser un double pointeur et faire la même manière que précédemment.


Petit rappel pour les pointeurs :

|accéder aux adresses mémoires à la **i** position|`(ptr + i)` = `&ptr[i]`|
|---------------------------------------------|-----------------------|
|accéder à l'adresse mémoire de la position actuelle|`(ptr)`|
|accéder aux valeurs des adresses mémoires à la **i** position|`(*(ptr + i))` = `ptr[i]`|
|accéder aux valeurs de l'adresse mémoire actuelle|`(*ptr)`|

---
Petit rappel pour les doubles pointeurs :

|accéder aux adresses mémoires à la **i** position|`((*double_ptr) + i)` = `&(*double_ptr)[i]`|
|---------------------------------------------|-----------------------|
|accéder à l'adresse mémoire de la position actuelle|`(*double_ptr)`|
|accéder aux valeurs des adresses mémoires à la **i** position|`(*((*double_ptr) + i))` = `(*double_ptr)[i]` = `double_ptr[k][i]`|
|accéder aux valeurs de l'adresse mémoire actuelle|`(**double_ptr)`|

---
Les pointeurs de structure permettent d'accéder aux éléments d'une structure via deux manière :
1. > (adresse mémoire)->élément | (ptr)->élément
2. > (valeur).élément           | (*ptr).élément

Petit rappel pour les pointeurs de structure

|accéder aux élément à la **i** position du pointeur de structure|`(*(ptr + i)).élément` = `ptr[i].élément` = `(ptr + i)->élément`|
|---|---|
|accéder aux élément à la position actuelle du pointeur de structure | `(ptr)->élément` = `(*ptr).élément`|
|accéder aux adresses mémoires à la **i** position du pointeur de structure|`&(ptr + i)->élément` = `&ptr[i].élément` = `&(*(ptr + i)).élément`|
|accéder aux adresses mémoires à la position actuelle du pointeur de structure|`&(ptr)->élément` = `&(*ptr).élément`|

---
Petit rappel pour les doubles pointeurs de structure

|accéder aux élément à la **i** position du double pointeur de structure|`(*((*double_ptr) + i)).élément` = `(*double_ptr)[i].élément` = `((*double_ptr) + i)->élément`|
|---|---|
|accéder aux élément à la position actuelle du double pointeur de structure | `(*double_ptr)->élément` = `(**double_ptr).élément`|
|accéder aux adresses mémoires à la **i** position du double pointeur de structure|`&((*double_ptr) + i)->élément` = `&(*double_ptr)[i].élément` = `&(*((*double_ptr) + i)).élément`|
|accéder aux adresses mémoires à la position actuelle du double pointeur de structure|`&(*double_ptr)->élément` = `&(**double_ptr).élément`|
