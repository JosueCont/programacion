##include <iostream>
#include <math.h>
using namespace std;

int main()
{
    int opcion,num,fac=1;
    float e,ex;        
    cout<<"MENU";
     cout<<"\n1.-valor constante";
     cout<<"\n2.-valor de ex";
     cout<<"\n3.-Salir";
     cout<<"\nElige una opcion:";
     cin>>opcion;
     
     
     
     if(opcion==1)
     {
         cout<<"Ingresa un numero:";
         cin>>num;
         for(int i=2;i<=num;i++)
         {
             cout<<fac<<"X"<<i<<"="<<fac*i<<"\n";
             fac*=i;
             e=1.0+1.0/fac*i;
           
         }
         cout<<"La constante es:"<<e;
         
         
     }
     
     if(opcion==2)
     {
         cout<<"Ingresa un numero:";
         cin>>num;
         for(int i=2;i<=num;i++)
         {
             cout<<fac<<"X"<<i<<"="<<fac*i<<"\n";
             fac*=i;
             ex=(pow(num,fac*i))/(fac*i)+1;
             
             
         }
         cout<<"valor de ex:"<<ex;
         
     }
     if(opcion==3)
     {
      do{
          cout<<"Quieres salir?1/0";
          cin>>opcion;
      }while(opcion!=1);
     }
  
    return 0;
}
