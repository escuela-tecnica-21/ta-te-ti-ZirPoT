# ta-te-ti-ZirPoT
ta-te-ti-ZirPoT created by GitHub Classroom
#include <stdio.h>
#include <stdlib.h>

void mostrarTablero(char tablero[]);
int Jugada();
void inicializarTablero(char tablero[]);
int comprobar_victoria();


char tablero [9];
int i,ficha_elegida,lugar_ocupado[9],eleccion=1,victoria_x=0,victoria_o=0;

int main() //programa principal
{
    void inicializarTablero(tablero);

    while(1)
    {
        system("cls");//borra la pantalla
       mostrarTablero(tablero);

       printf("Que ficha quiere jugar?   1-X    2-O   3-TERMINAR\n");
       scanf("%d",&ficha_elegida);

       if(ficha_elegida==1)
       {
         Jugada();
         if(lugar_ocupado[eleccion-1]==0)
         {
           tablero[(eleccion-1)] = 'X';//en la posicion elegida pone una X
           lugar_ocupado[eleccion-1]=1; //ocupa el lugar con un 1
         }

       }

       if(ficha_elegida==2)
       {
         Jugada();
         if(lugar_ocupado[eleccion-1]==0)
         {
           tablero[(eleccion-1)] = 'O';//en la posicion elegida pone una O
           lugar_ocupado[eleccion-1]=2;
         }
       }
       comprobar_victoria();
       if(ficha_elegida==3)
       {
           break;
       }
       lugar_ocupado;
       if(victoria_x==1)
       {

           printf("Gana las x");
           break;
       }

       for(i=0;i<9;i++)
       {

           printf("%d",victoria_x);

       }
    }


    return 0;
}
//funciones
void mostrarTablero(char tablero[])//funcion que dibuja el tablero
{
    printf(" %C | %C | %C\n", tablero[0], tablero[1], tablero[2]);
    printf("---|---|---\n");
    printf(" %C | %C | %C\n", tablero[3], tablero[4], tablero[5]);
    printf("---|---|---\n");
    printf(" %C | %C | %C\n", tablero[6], tablero[7], tablero[8]);
    printf("\n");
    return;
}

int Jugada()
{
    eleccion=0;
    while(eleccion<1 || eleccion>9) //sale del while si es correcta la posicion
    {
       printf("Elegi un posicion para jugar del 1 al 9\n");
       scanf("%d",&eleccion);
       if(eleccion<1 || eleccion>9)
       {
           printf("Solo se puede jugar del 1 al 9\n");
       }
    }

 return eleccion-1;
}

void inicializarTablero(char tablero[])//llena la matriz del tablero
{
    for (int i=0; i < 9; i++){
        tablero[i]=' ';
        lugar_ocupado[i]=0;
    }
    return;
}

int comprobar_victoria()
{
    if(lugar_ocupado[0]==1 && lugar_ocupado[1]==1 && lugar_ocupado[2]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[3]==1 && lugar_ocupado[4]==1 && lugar_ocupado[5]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[6]==1 && lugar_ocupado[7]==1 && lugar_ocupado[8]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[0]==1 && lugar_ocupado[3]==1 && lugar_ocupado[6]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[1]==1 && lugar_ocupado[4]==1 && lugar_ocupado[7]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[2]==1 && lugar_ocupado[5]==1 && lugar_ocupado[8]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[0]==1 && lugar_ocupado[4]==1 && lugar_ocupado[8]==1 )
    {
      victoria_x=1;
    }
    if(lugar_ocupado[2]==1 && lugar_ocupado[4]==1 && lugar_ocupado[6]==1 )
    {
      victoria_x=1;
    }
}
