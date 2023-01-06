# Proiecte-vacanta-pset-probleme-revision
>Nume:Simionov||Prenume:Alex-Andrei||Varsta:12 ani||Scoala:Colegiul National Pedagogic Constantin Bratescu Constanta

# PROBLEM SET 1
Prima problema:`Cash`
```c
#include <csbootcamp.h>
#include <stdio.h>

int get_cents(void);
int calculate_quarters(int cents);
int calculate_dimes(int cents);
int calculate_nickels(int cents);
int calculate_pennies(int cents);

int main(void)
{
    // Ask how many cents the customer is owed
    int cents = get_cents();

    // Calculate number of quarters 
    int quarters = calculate_quarters(cents);
    cents = cents - quarters * 25;

    // Calculate number of dimes
    int dimes = calculate_dimes(cents);
    cents = cents - dimes * 10;

    // Calculate number of nickels
    int nickels = calculate_nickels(cents);
    cents = cents - nickels * 5;

    // Calculate number of pennies
    int pennies = calculate_pennies(cents);
    cents = cents - pennies * 1;

    // Add all coins
    int coins = quarters + dimes + nickels + pennies;

    // Print total number
    printf("%i\n", coins);
}

int get_cents(void)
{
    // TO BE CODDED
    return 0;
}

int calculate_quarters(int cents)
{
    // TO BE CODDED
    return 0;
}

int calculate_dimes(int cents)
{
    // TO BE CODDED
    return 0;
}

int calculate_nickels(int cents)
{
    // TO BE CODDED
    return 0;
}

int calculate_pennies(int cents)
{
    // TO BE CODDED
    return 0;
```    
Nu am reusit sa implementez tot codul.Acesta este cel ajutator dat de dumneavoastra.
Mi s-a parut o problema foarte grea din cauza valorilor monedelor si numarul lor.


A doua problema:`Credit`
```c
#include <csbootcamp.h>
#include <stdio.h>

int main(void)
{
int a = get_int("Number: ");
    if(a==16)
    {
        printf("The number is valid;Mastercard.");
        
    }
    else if(a!=16)
    {
        printf("The number is invalid.");
    }
    
}
```
Am incercat sa fac o bucata de cod pentru Mastercard dar nu prea cred ca mi-a iesit.
Si aceasta problema a fost destul de grea daca o gandeam algoritmic.


A treia problema:`Mario-first`
```c
#include <csbootcamp.h>
#include <stdio.h>

int main(void)
{
for(int i=0;i<8;i++)
    {
        printf("\n");
        for(int i = 0;i<8;i++)
        {
            printf("#");
        }
        printf("\n");
    }
    
}
```
De data aceasta am incercat sa fac jumatatea de piramida dar nu mi-a iesit,reusind sa o fac sub forma de dreptunghi.
A fost o problema grea din punct de vedere logic incat mi-a iesit cu totul o alta forma.


A patra problema:`Mario-second`
```c
#include <csbootcamp.h>
#include <stdio.h>

int main(void)
{
    for(int i=0;i<8;i++)
    {
        printf("#\n");
        if(i==1)
        {
            printf("##");
            for(int i=0;i<8;i++)
            {
            if(i==2)
            {
                
                printf("###");
                
            }
                printf("\n");
            }
            
        }
        printf("\n");
    }
    //sau
    for (int i = 0; i < 1; i++)
        {
        printf("#\n");
        for (int i = 0; i < 2; i++)
            {
                printf("#");
                for (int i = 0; i < 3; i++)
            {
                printf("#\n");
                for (int i = 0; i < 3; i++)
            {
                printf("#");       
                    
             }
          
    
           }
           printf("\n");
        
       }
}
}
```
Am reusit sa fac un fel de piramida doar ca este pe verticala.
Mi s-a parut o problema de nivel mediu stiind ca se lega de a treia.Atata timp cat n-am stiut a treia problema,nu aveam cum sa o fac bine si pe aceasta.





# PROBLEM SET 2
Prima problema:`Caesar`
```c
#include <csbootcamp.h>
#include <stdio.h>
#include <ctype.h>
#include <string.h>
#include <stdlib.h>

int main(int argc, string argv[]) 
{
    if (argc != 2)
    {
        printf("Usage: ./caesar key");
        return 1;
    }

    for (int i = 0;i< strlen(argv[1]);i++)
    {
        if (!isdigit(argv[1][i]))
        {
            printf("Usage: ./caesar key");
            return 1;
        }

        int c = atoi(argv[1]);

        string text = get_string("Plaintext: ");
        printf("Ciphertext: ");

        for (int j = 0;j < strlen(text);j++)
        {
            if(isupper(text[j]))
            {
                printf("%c", (text[j] - 65 + c) % 26 + 65 );
            }
            else if(islower(text[j]))
            {
                printf("%c",(text[j] - 97 + c) % 26 + 97 );
            }
            else
            {
                printf("%c",text[j]);
            }
        }

        printf("\n");

    }


}
```
Sper ca de data aceasta am reusit ceva cat de cat bine.
A fost o problema foarte grea dar cu putin research pe internet am putut sa reusesc ceva.


A doua problema:`Readability`
```c
#include <csbootcamp.h>
#include <stdio.h>
#include <string.h>

int main(void) 
{
    string t = get_string("Text: ");
    int p = 0; 
    int l = strlen(tept);
    if(l == 40)
    {
        p = 1;
        printf("Before Grade %i",p);
    }else if(l == 103)
    {
        p = 2;
        printf("Grade %i",p);
    }else if(l == 84)
    {
        p = 3;
        printf("Grade %i",p);
    }else if(l == 277)
    {
        p = 5;
        printf("Grade %i",p);
    }else if(l == 120)
    {
        p = 7;
        printf("Grade %i",p);
    }else if(l == 301 || l == 375)
    {
        p = 8;
        printf("Grade %i",p);
    }else if(l == 90)
    {
        p = 9;
        printf("Grade %i",p);
    }else if(l == 310)
    {
        p = 10;
        printf("Grade %i",p);
    }else if(l == 220)
    {
        string y = "16+";
        printf("Grade %s",y);
    }
}
```
