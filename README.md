#include <iostream>
#include <conio.h>
#include "coordenadas.h""
using namespace std;

void entrada(int V[ ],int lim, int col, int fil);

main (){
	int V1[4],V2[4],V3[4],V4[4],V5[4],V6[4],V7[4],V8[4];
	    gotoxy(6,1);cout<<"SUMA";
	entrada (V1,4,5,3);
	gotoxy(2,4);cout<<"+";
	entrada (V2,4,5,4);
		gotoxy(30,1);cout<<"RESTA";
	entrada (V3,4,30,3);
	gotoxy(28,4);cout<<"-";
	entrada (V4,4,30,4);
		gotoxy(6,9);cout<<"MULTIPLICACION";
	entrada (V5,4,5,10);
	gotoxy(2,11);cout<<"x";
	entrada (V6,4,5,11);
		gotoxy(30,9);cout<<"DIVISION";
	entrada (V7,4,30,10);
		gotoxy(28,11);cout<<"/";
	entrada (V8,4,30,11);
	getch();
}

void entrada (int V[ ],int lim,int col,int fil){
int x;
	for(x=0;x<lim;x++){
		gotoxy(col+(x*4),fil); cin>>V[x];
	}
}
