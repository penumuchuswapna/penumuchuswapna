#include <stdio.h>

   int strcmp(char s[],char t[]);


 void main()
 {

    char s[20],t[20];
   printf("Type in a string s.\n");
   gets(s);
    printf("Type in a string t.\n");
    gets( t );
   printf("The result of comparison=%d\n",strcmp(s,t));

    return 0;
      }


   int strcmp(char s[],char t[])
  {
   int i;
   for(i=0;s[i]==t[i];i++)
   if(s[i]=='\0')
   return( 0 );
   return(s[i]-t[i]);
   }
