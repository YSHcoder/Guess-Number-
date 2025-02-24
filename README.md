#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main (){
    int random,guess;
    int no_of_guess =0;
    srand(time(NULL));


   printf("Welocme to the world of guessing a number:\n");
   random = rand() % 100 + 1; // Generating between 0 to 100                   

   do{
    printf("Please enter a number between(1 to 100):\n");
    scanf("%d",&guess);
    no_of_guess++;

    if (guess < random ){
        printf("Guess a larger number.\n");
    }else if(guess > random){
        printf("Guess a smaller number.\n");
    }
    else{
        printf("Congratulation !!! You have sucessfully guessed the number.\n");
    }
   }while(guess != random);

   printf("Bye Bye, Thank you for playing.\n ");
   printf("Developed by Yash");


}


