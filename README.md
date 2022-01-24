# code-dump

//program to merge two unsorted arrays

      #include <stdio.h>

      void Merge_US(int x[], int y[]){
          int c[10],i,j,k;
          for(i=0,k=0;i<5;i++,k++){
              c[k] = x[i];
          }

          for(k,j=0; k<10,j<5;k++,j++){
              for(i=0;i<5;i++){
                  if(c[i] == y[j])
                      continue;
                  else
                      c[k] = y[j];
              }
          }

          for(int i=0;i<10;i++)
              printf("%d  ",c[i]);
      }

      int main()
      {
          int a[] = {3,12,15,17,20};
          int b[] = {2,5,7,9,22};

          int a1[] = {78,0,45,17,20};
          int b1[] = {16,9,7,20,50};

          Merge_US(a1,b1);
          printf("Hello World");

          return 0;
      }
      
      
 
