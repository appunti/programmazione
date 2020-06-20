# Variabili e Costanti

Nella programmazione le variabili rappresentano **valori che possono cambiare**. In alternativa esistono le costanti. Queste ultime ci permettono di specificare dei dati che non possono essere cambiati durante l'esecuzione del programma.

Le variabili si possono vedere come dei "contenitori" (piccole aree di memoria riservate) che contengono un dato.

Quando si programma in Java (linguaggio di programmazione fortemente tipizzato), oltre al nome della variabile o della costante, bisogna specificare anche il tipo di dato.

## Tipologia delle Variabili

Il linguaggio di programmazione Java ci mette a disposizione delle tipologie di variabili "elementari" che possiamo utilizzare per scrivere i nostri programmi.

Tra i tipo predefiniti abbiamo:

| Tipo | Utilizzo |
|---|---|
| `int` | Rappresenta numeri interi |
| `char` | Rappresenta caratteri alfanumerici |
| `String` | Rappresenta sequenze di caratteri |
| `double` | Rappresenta numeri in doppia precisione |
| `float` | Rappresenta numeri in virgola mobile |
| `boolean` | Rappresenta valori booleani (0 oppure 1) |

## Definizione di una variabile

Per definire una variabile si possono usare le seguenti notazioni:

1. **Definizione**:
    ```
    <tipo> <nome>;
    ```
    Esempio:
    ```java
    int conteggio;
    ```
2. **Definizione ed assegnazione**:
    ```
    <tipo> <nome> = <valore>;
    ```
    Esempio:
    ```java
    String nome = "Antonella";
    ```

## Operazioni con le Variabili

Con le variabili possiamo fare principalmente due operazioni:
- Assegnazione;
- Lettura.

Le operazioni di assegnazione vengono svolte usando il simbolo "`=`" posto tra il nome della variabile e il nuovo valore da assegnare.

Esempio:

```java
float raggio = 3;
float areaCerchio;
areaCerchio = 3.14159265 * Math.pow(raggio, 2);
```
Le operazioni di lettura, invece avvengono specificando il nome della variabile da leggere.

Esempio:

```java
float raggio = 3;
float areaCerchio = 3.14159265 * Math.pow(raggio, 2);
System.out.print("L'area del cerchio è: ");
System.out.println(areaCerchio);
```

## Definizione di Costanti

In un modo molto simile alle Variabili si possono definire le costanti, basta anteporre la parola `final` prima della dichiarazione e assegnazione.

Esempio:

```java
final float piGreco = 3.14159265;
float raggio = 3;
float areaCerchio = piGreco * Math.pow(raggio, 2);
System.out.print("L'area del cerchio è: ");
System.out.println(areaCerchio);
```
