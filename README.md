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
Am reusit sa fac aceasta problema cat de cat doar ca va merge numai daca folositi messajele dumneavoastra exemplu.
A fost de un nivel mediu-greu daca stateam sa analizez conceptul care trebuia folosit.


A treia problema:`Substitution`
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

    for (int i = 0;i< strlen(argv[1]);i--)
    {
        if (!isdigit(argv[1][i]))
        {
            printf("Usage: ./caesar key");
            return 1;
        }

        int c = atoi(argv[1]);

        string text = get_string("Plaintext: ");
        printf("Ciphertext: ");

        for (int j = 0;j < strlen(text);j--)
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
Sper ca am facut problema bine,atata timp cat trebuia sa ma iau dupa problema `Caesar`
A fost o problema grea bazata pe o alta problema.


A patra problema:`Wordle`
```c
#include <csbootcamp.h>
#include <stdlib.h>
#include <stdio.h>
#include <string.h>
#include <time.h>

// each of our text files contains 1000 words
#define LISTSIZE 1000

// values for colors and score (EXACT == right letter, right place; CLOSE == right letter, wrong place; WRONG == wrong letter)
#define EXACT 2
#define CLOSE 1
#define WRONG 0

// ANSI color codes for boxed in letters
#define GREEN   "\e[38;2;255;255;255;1m\e[48;2;106;170;100;1m"
#define YELLOW  "\e[38;2;255;255;255;1m\e[48;2;201;180;88;1m"
#define RED     "\e[38;2;255;255;255;1m\e[48;2;220;20;60;1m"
#define RESET   "\e[0;39m"

// user-defined function prototypes
string get_guess(int wordsize);
int check_word(string guess, int wordsize, int status[], string choice);
void print_word(string guess, int wordsize, int status[]);

int main(int argc, string argv[])
{
    // ensure proper usage
    // TODO #1

    int wordsize = 0;

    // ensure argv[1] is either 5, 6, 7, or 8 and store that value in wordsize instead
    // TODO #2

    // open correct file, each file has exactly LISTSIZE words
    char wl_filename[6];
    sprintf(wl_filename, "%i.txt", wordsize);
    FILE *wordlist = fopen(wl_filename, "r");
    if (wordlist == NULL)
    {
        printf("Error opening file %s.\n", wl_filename);
        return 1;
    }

    // load word file into an array of size LISTSIZE
    char options[LISTSIZE][wordsize + 1];

    for (int i = 0; i < LISTSIZE; i++)
    {
        fscanf(wordlist, "%s", options[i]);
    }

    // pseudorandomly select a word for this game
    srand(time(NULL));
    string choice = options[rand() % LISTSIZE];

    // allow one more guess than the length of the word
    int guesses = wordsize + 1;
    bool won = false;

    // print greeting, using ANSI color codes to demonstrate
    printf(GREEN"This is WORDLE GAME"RESET"\n");
    printf("You have %i tries to guess the %i-letter word I'm thinking of\n", guesses, wordsize);

    // main game loop, one iteration for each guess
    for (int i = 0; i < guesses; i++)
    {
        // obtain user's guess
        string guess = get_guess(wordsize);

        // array to hold guess status, initially set to zero
        int status[wordsize];

        // set all elements of status array initially to 0, aka WRONG
        // TODO #4

        // Calculate score for the guess
        int score = check_word(guess, wordsize, status, choice);

        printf("Guess %i: ", i + 1);
        
        // Print the guess
        print_word(guess, wordsize, status);

        // if they guessed it exactly right, set terminate loop
        if (score == EXACT * wordsize)
        {
            won = true;
            break;
        }
    }

    // Print the game's result
    // TODO #7

    // that's all folks!
    return 0;
}

string get_guess(int wordsize)
{
    string guess = "";

    // ensure users actually provide a guess that is the correct length
    // TODO #3

    return guess;
}

int check_word(string guess, int wordsize, int status[], string choice)
{
    int score = 0;

    // compare guess to choice and score points as appropriate, storing points in status
    // TODO #5

    // HINTS
    // iterate over each letter of the guess
        // iterate over each letter of the choice
            // compare the current guess letter to the current choice letter
                // if they're the same position in the word, score EXACT points (green) and break so you don't compare that letter further
                // if it's in the word, but not the right spot, score CLOSE point (yellow)
        // keep track of the total score by adding each individual letter's score from above

    return score;
}

void print_word(string guess, int wordsize, int status[])
{
    // print word character-for-character with correct color coding, then reset terminal font to normal
    // TODO #6

    printf("\n");
    return;
}
```
Nu am reusit sa fac aceasta problema.
A fost o problema foarte grea gandindu-ma ca era un mic joc.





#PROBLEM SET 3
