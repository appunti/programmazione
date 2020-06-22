# Metodi e Classi

In Java (e più generalmente nella programmazione ad oggetti), le classi sono le entità che hanno il compito di rappresentare gli oggetti.
Ogni classe può contenere da 0 a più metodi, questi ultimi vengono utilizzati per fare operazioni su dati interni e/o esterni alla classe.

Ogni programma Java deve contenere almeno una classe, e, per essere eseguito deve avere almeno un metodo `main`.

Per definire una classe abbiamo bisogno di specificare il nome della stessa e come le altre classi ci possono interagire (i modifiers).

Normalmente nelle classi troviamo gli access modifiers che sono:

| Nome | Funzione |
|---|---|
| `public` | Rende la classe visibile a tutte le altre classi del programma |
| `private` | Rende la classe visibile solo alla classe direttamente all'esterno |

## Esempi di classe

- Classe public con metodo main che stamperà "Ciao mondo":
    ```java
    public class Prova {
        private String cosa = "mondo";
        public static void main(String[] args) {
            System.out.println("Ciao " + cosa);
        }
    }
    ```
- Classe private dentro classe public con metodo che interagisce con la classe private:
    ```java
    public class Provola {

        public static boolean isFormaggio() {
            return Formaggio.isFormaggio();
        }

        private static class Formaggio {
            public static boolean isFromaggio() {
                return true;
            }
        }
    }
    ```

## Metodi

I metodi ci permettono di separare il codice in modo più specifico e separarlo in unità di codice riutilizzabile.
