#include <stdio.h>
#include <math.h>
#include <stdlib.h>


void phonenumber(int *phone)
{
    int i=0;
    printf("Please enter a seven digit phone number\n");

    for(i=0; i<7; i++)
    {
        scanf("%d", phone+i);
    }

}



void main()
{

    int phone[7]={1,2,2,2,2,5,3};
    phonenumber(phone);
    int numbers[]={phone[3], phone[4], phone[5], phone[6]};


    char two[]="abcc", three[]= "deff", four[]="ghii", five[]="jkll", six[]="mnoo", seven[]=    "pqrs",    eight[]=    "tuvv", nine[]="wxyz";




    char *code[] = {two,three,four,five,six,seven,eight,nine};

    char *xpos[]= {two,three,four,five};

    int i,j,k,n,b,c,f,q,d, flag;
    for(i=0;i<4;i++)
    {
        for(j=0;j<8;j++)
        {
            if(numbers[i]==j+2)
            {
                xpos[i] = code[j];

            }
        }
    }


    for(j=0;j<4;j++)
    {
            for(n=0;n<4;n++)
            {
                for(c=0;c<4;c++)
            {
                for(q=0;q<4;q++)
            {


                char str1,str2,str0,str3;

                str0= xpos[0][j];
                str1= xpos[1][n];
                str2= xpos[2][c];
                str3= xpos[3][q];
                char word[5] ={str0,str1,str2,str3};

                //printf("%s\n", word);

                FILE *words;
                words = fopen("C:\\EnglishWords4Letters.txt" ,"r");

                for(d=0; d<500; d++)
                        {

                            char x[5];
                            fscanf(words, "%4s", x);
                            //printf("%s\n", x);

                            flag=strcmp(x,word);
                            if(flag==0)
                            {
                                char trans[5];
                                printf("The translation of the last four letters: %s", word);
                                return 1;
                            }

                        }
                fclose(words);
                }
            }

            }

    }

printf("translation failed");

return 0;
}
