# Ejercicio: Lista Linkeada Invertida

## Instrucciones

Utilizando como base las clases *Linked List* y *Stack* que se encuentran en el Gist, realizar las siguientes modificaciones:

**Reverse Inplace:** este método debe incluirse en la clase Linked List, su funcionalidad consiste en invertir el orden de la lista simplemente ligada a través de modificaciones en los punteros. Este método no requiere ningún retorno específico, ya que modifica la instancia original de la lista.

Para implementarlo, debe basarse en el siguiente pseudocódigo: 

> REVERSE_IN_PLACE():
>
>
> IF START == NIL:  
> &nbsp;&nbsp;&nbsp;&nbsp;EMPTY LIST  
> 
> SET CURRENT_NODE = START  
> SET PREV_NODE = NIL  
> SET NEXT_NODE = NIL  
> 
> WHILE CURRENT_NODE != NIL:  
>&nbsp;&nbsp;&nbsp;&nbsp;SET NEXT_NODE = CURRENT_NODE.NEXT  
>&nbsp;&nbsp;&nbsp;&nbsp;SET CURRENT_NODE.NEXT = PREV_NODE  
>&nbsp;&nbsp;&nbsp;&nbsp;SET PREV_NODE = CURRENT_NODE  
>&nbsp;&nbsp;&nbsp;&nbsp;SET CURRENT_NODE = NEXT_NODE 
>  
>SET START = PREV_NODE

## Testing

Para evaluar el funcionamiento de su código, deberá realizar lo siguiente en el archivo `test.py`:

1) Crear una instancia de Linked List y agregar 10 elementos en ella.
2) Imprimir la lista original.
3) Imprimir ambas listas resultantes para evaluar que sean iguales.

## Results
 ![Console results](https://github.com/PhilipFalla/Resersed-LL/blob/main/img/result_console.png)