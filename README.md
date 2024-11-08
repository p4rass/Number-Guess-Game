//GUESS THE NUMBER



#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main(){
    srand(time(0));
    int r = (rand()%10) + 1;
    printf("guess a number between 1 to 10\n");
    int b = 1;   
    while (1 < 2){
        int a;
        scanf("%d", &a);
        if (a == r){
            printf("hurray, you got it right\n");
            break;
            b++;
        }
        else if (a < r){
            printf("chose a number greater then %d\n", a);
            b++;
        }    
         else if (a > r){
            printf("chose a number lower then %d\n", a);
            b++;
        }    
        }
    printf("you gussed the number in %d attempts", b);    
    return 0;
    }
    
