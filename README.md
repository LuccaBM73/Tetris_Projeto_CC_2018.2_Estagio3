#include <stdio.h>
#include <stdlib.h>
#include <math.h>
#include <stdbool.h>
#include <string.h>



int primo(){
  
  int i, x; 
  int div = 0;
  
  do {
    printf("Digite um numero inteiro e positivo: ");
    scanf("%d", &x);
  } while (x <= 0);
  
  for (i = 1; i <= x; i++) {
    if (x % i == 0) { 
     div++;
    }
  }
    
  if (div == 2)
    printf("O numero %d e primo!\n", x);
  else
    printf("O numero %d nao e primo!\n", x);

}
	int fat(){
	
	
    
	
    int cavalo,jumento;
    printf("Insira um valor para o qual deseja calcular seu fatorial: ");
    scanf("%d", &jumento);
    for(cavalo=1; jumento>1; jumento=jumento-1)
    cavalo=cavalo*jumento;
    printf("\nFatorial calculado: %d\n", cavalo);
}
int primo2(){
	int n;
	do{ 
		primo();
	}
	while(n==0);
	
}

float flutuante5(){


float N1,N2,potencia,raiz;
printf("Digite o numero e depois a potencia: ");
scanf("%f",&N1);
scanf("%f",&N2);

potencia=pow(N1,N2);

raiz=sqrt(N1);

printf("Quadrado do numero=%f\n",potencia);





}

float Raiz1(){

}

int ano(){

	int ano;
	bool bissexto;
 
	
	printf("Digite o ano: ");
 
	
	scanf("%d", &ano);
 
	if (ano % 400 == 0) {
		bissexto = true;		
	}
	else if ((ano % 4 == 0) && (ano % 100 != 0)) {
		bissexto = true;		
	}
	else {
		bissexto = false;
	}
 
	if (bissexto == true) {
		printf("O ano e bissexto!\n");
	} else {
		printf("O ano nao e bissexto!\n");
	}
}

float nota(){
 float n1,n2,media ;
 
     
                                
   printf("Qual a nota do primeiro teste: ");
   scanf("%f", &n1);
   printf("Qual a nota do segundo teste: ");
   scanf("%f", &n2);
    if(n1,n2>=0 && n1,n2<=10) {
	         
   		media=(n1+n2)/2;   
  		 printf("%f\n",media) ; }
    else {
	
   		printf("Nota invalida\n");          
}
          }
float nota2(){
 float n1,n2,n3,x,media ;	
	
   printf("Qual a nota do primeiro teste: ");
   scanf("%f", &n1);
   printf("Qual a nota do segundo teste: ");
   scanf("%f", &n2);
   printf("Qual a nota do terceiro teste: ");
   scanf("%f", &n3);
   if (n1>n2){
   			x=n1;
   			printf("sua media é %f\n",(x+n3)/2);
		}
   	else{
   			x=n2;
   			printf("sua media é %f\n",(x+n3)/2);
	   }
	   
}

int matricula(){
		int numeroEntrada, q, resto;
	char exa[10], getInt[10];
	
	printf("Informe um numero para converter para HEXADECIMAL\n\n");
	printf("NUMERO :\n ");
	scanf("%i", &numeroEntrada);
	
	
		do{
		q = numeroEntrada / 16;
		resto = numeroEntrada % 16;
		numeroEntrada /= 16;
		
		switch(resto){
			case 10:
				strcat(exa, "A");
			break;
			case 11:
				strcat(exa, "B");
			break;
			case 12:
				strcat(exa, "C");
			break;
			case 13:
				strcat(exa, "D");
			break;
			case 14:
				strcat(exa, "E");
			break;
			case 15:
				strcat(exa, "F");
			break;
			case 16:
				strcat(exa, "G");
			break;
			default:
				sprintf(getInt, "%i", resto);
				strcat(exa, getInt);
		}
	}while(q != 0);
	printf("%s\n\n", exa);
	return 0;
	
}




/*___________________________________________________________________________________________________________________________________________
	|																																	|
		|						  L								B	B	B	B	B					M				M				|
	|							L	L							B								M		M		 M		M		|
		|						L	L							B				B				M		 M		M		M			|
	|							L	L							B				B				M		 M		M		M		|
		|						L	L							B				B				M		 M	 	M		M			|
	|							L	L							B				B				M		 M		M		M		|
		|						L	L							B	B	B	B					M		 M		M		M			|
	|							L	L							B	B	B	B					M		 M		M		M		|
		|						L	L							B				B				M		 M		M		M			|
	|							L	L							B				B				M		 M	M	M		M		|																																|
		|						L	L							B				B				M						M			|																															
	|							L	L	L	L	L	L			B				B				M						M		|
		|						L	L	L	L	L	L			B	B	B	B	B   			M						M			|
_______________________________________________________________________________________________________________________________________________	*/	







int main(){

			int a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,x,y,z;
			
			do{
			
			
				printf("|OPCAO 1 -solicitar fatorial|\n");
				printf("|OPCAO 2 - primo?,nprimo?|\n");
				printf("|OPCAO 3 - primo que retorna|\n");
				printf("|OPCAO 4 - potencia top|\n");
				printf("|OPCAO 5 - xxxxxxxxxx|\n");
				printf("|OPCAO 6 - bissexto?|\n");
				printf("|OPCAO 7 - nota|\n");
				printf("|OPCAO 8 - nota2|\n");
				printf("|OPCAO 9 -matricula|\n");
				printf("|OPCAO 0 - Para fechar|\n");
				scanf("%d",&a);
				switch (a)
					{
					case 1:fat()	;break;
					case 2:primo()	;break;
					case 3:primo2();break;
					case 4:flutuante5();break;
					case 5:	printf("OPCAO INEXISTENTE: %d\n",a);break;
					case 6:	ano();break;
					case 7:	nota();break;
					case 8:	nota2();break;
					case 9:	matricula();break;
					case 0:	printf("ADIOS AMIGO :): %d\n",a);break;
					}
			}	
			while(a!=0);
	

}
