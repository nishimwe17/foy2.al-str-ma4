#include <stdio.h>
#include <stdlib.h>
int main(int argc, char *argv[])
{
  int alt_sinir, ust_sinir, toplam, i;
  alt_sinir = atoi(argv[1]);
  ust_sinir = atoi(argv[2]);
  printf("%d ile %d arasindaki sayilarin toplami : ", alt_sinir, ust_sinir);
  i = alt_sinir;
  
  etiket1:
   toplam = toplam + i;
   i++;
   if (i<=ust_sinir)
  goto etiket1;

  printf("%d\n", toplam);
  return 0;
}
