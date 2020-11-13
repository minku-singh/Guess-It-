# Guess-It-
//You have to guess the number and it will tell you in how many attempts you have guessed it.
//guess game
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main()
{
    int number,guess,nguess=1;
    srand(time(0));
    number= rand()%100 +1;
    //printf("Random number: %d \n",number);

   do
    {
      printf("Guess the number: ");
      scanf("%d",&guess);
      if(guess>number)
       {
        printf("Enter smaller number!! \n");
       }
       else if(guess<number)
       {
           printf("Enter bigger number!! \n");
       }
       else
       {
           printf("You Guessed in %d attempts!!",nguess);
       }
       nguess++;
    }
    
    while(number!=guess);
    
    
}
