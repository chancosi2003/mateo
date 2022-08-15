#include <iostream>
#include <conio.h>
#include <string.h>
using namespace std;
int main(){
    char h[10], g[10], j[10];
    int i=1;
    cout<<"ingrese una cadena\n";
    cin.getline(g,10,'\n');
    cout<<"la cadena ingresada es: "<<g<<"\n";
    h[0]=g[0];
    h[1]='\0';
    while (g[i]!='\0')
    {
        j[i-1]=g[i];
        i++;
    }
    
    strupr(h);
    strcat(h,j);
    cout<<"La cadena modificada es: "<<h<<"\n";
     string mars=" ";
      for(int i=0;i<mars.length();i++){
        if((mars[i]!=' ' && h[i+1]!=' ')){
            i=i+1;
        }
    }
    cout<< "hay "<<i<<" digitos "<<endl;
    return 0;

}

