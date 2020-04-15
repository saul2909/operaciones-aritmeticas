#include<iostream>
#include<conio.h>
using namespace std;

double suma(double x, double y);
double resta(double x, double y);
double multiplicacion(double x, double y);
double division(double x, double y);

int main(){

	double x,y,res;
	int opc;
	cout<<"ingresa el Numero 1: \n";
	cin>>x;
	cout<<"ingresa el Numero 2: \n";	
	cin>>y;	
	
	
	
	cout<<"Seleccione un Numero\n";
		cout<<"1.-Suma\n";
		cout<<"2.-Resta\n";
		cout<<"3.-Multiplicacion\n";
		cout<<"4.-Division\n";
		cin>>opc;
	
	
		switch(opc){
		
		case 1:
		    res = suma(x,y);//funcion sumar
		cout<<"El resultado es: "<<res;	
		
		break;
		
		case 2:
			res = resta(x,y);//funcion resta
		cout<<"El resultado es: "<<res;
		
		break;
		
		case 3:
			res = multiplicacion(x,y);//funcion multiplicacion
		cout<<"El resultado es: "<<res;
		
		break;
		
		case 4:
			res = division(x,y);//funcion dividir
		cout<<"El resultado es: "<<res;
		
		break;
			
		default:
			cout<<"Opcion Incorrecta\n";
	}//fin del switch
	
		
		getch();
		return 0;	
	}//fin del main
	
	double suma(double x, double y){//Declarada directamente
	double res;//Declaracion de variable local
	res = x+y;//suma de manera local
	return res;//regresa el resultado de la suma, con la variable "res"
}

	double resta(double x, double y){//Declarada directamente
	double res;//Declaracion de variable local
	res = x-y;//resta de manera local
	return res;//regresa el resultado de la resta, con la variable "res"
}
	
	double division(double x, double y){//Declarada directamente
	double res;//Declaracion de variable local
	res = x/y;//divide de manera local
	return res;//regresa el resultado de la division, con la variable "res"
}

double multiplicacion(double x, double y){//Declarada directamente
	double res;//Declaracion de variable local
	res = x*y;//multiplica de manera local
	return res;//regresa el resultado de la multiplicacion, con la variable "res"
}
