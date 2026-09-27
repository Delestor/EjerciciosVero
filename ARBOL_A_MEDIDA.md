# Ejercicio: un árbol a medida

Vas a crear un programa en Java que dibuje la forma de un árbol de Navidad en la consola usando asteriscos (`*`).

El programa debe pedir al usuario un número entero llamado **altura**. Ese número indica cuántas filas tendrá el dibujo.

Por ejemplo, si el usuario introduce `4`, el resultado debe ser:

```text
   *
  ***
 *****
*******
```

## Reglas

- El dibujo debe tener tantas filas como indique la altura.
- La primera fila tiene un asterisco. Cada fila siguiente tiene dos asteriscos más que la anterior.
- Los asteriscos deben quedar centrados para formar un triángulo.
- Si la altura es menor que `1`, el programa debe mostrar un mensaje de error en lugar de dibujar el árbol.
- El dibujo debe construirse a partir del número introducido: no vale escribir un árbol distinto a mano para cada altura.
- **No hay que dibujar el tronco.**

Puedes probar también con altura `1`:

```text
*
```

Y con altura `3`:

```text
  *
 ***
*****
```

## Material permitido

Puedes usar variables, `String`, `if`/`else`, bucles `for` o `while`, y `System.out.print` / `System.out.println`.

Para leer la altura, puedes partir de este código; no hace falta que entiendas todavía todos sus detalles:

```java
import java.util.Scanner;

public class ArbolNavidad {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("¿Qué altura quieres para el árbol? ");
        int altura = scanner.nextInt();

        // Continúa aquí el programa.
    }
}
```
