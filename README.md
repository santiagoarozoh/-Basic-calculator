# -Basic-calculator
first calculator in C 
#include<stdio.h>
#include<math.h>
#include<stdlib.h> /* colaboration with joseph22106*/

int main(){
	
	int a,d; float b,c,ANS,e; 
	do{
	    printf("Digite el numero para elegir la operacion y digite los valores a operar\n");
	    printf("      MENU\n");
	    printf("-------------------------------\n");
	    printf("1.  SUMA\n");
	    printf("2.  RESTA\n");
	    printf("3.  MULTIPLICACION\n");     
	    printf("4.  DIVISION\n");
	    printf("5.  PORCENTAJE\n");
	    printf("6.  POTENCIA\n");
	    printf("7.  LOGARITMO\n");
	    printf("8.  SENO\n");
	    printf("9.  COSENO\n");
	    printf("10. TANGENTE\n");
    	printf("11. RAIZ CUADRADA\n");
    	printf("12. LIMPIAR PANTALLA\n");
    	printf("13. FINALIZAR PROGRAMA\n");
    	scanf("%i",&a);
    	if(a==12) system("cls");
    	switch(a) {
		    case 1: //printf("Digite los valores a sumar y pulse enter\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite el segundo numero\n");
		    	scanf("%f",&c);
		    	ANS=e+c;
		    	printf("La suma de %.2f y %.2f es: %.2f\n",e,c,ANS);
			}else{
			printf("Digite los valores a sumar y pulse enter\n");
			scanf("%f",&b);
		    scanf("%f",&c);
		    ANS=b+c;
		    printf("La suma de %.2f y %.2f es: %.2f\n",b,c,ANS);	
			}
		    e=ANS;
		    break;
		    case 2: //printf("Digite los valores a restar y pulse enter\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite el segundo numero\n");
		    	scanf("%f",&c);
		    	ANS=e-c;
		    	printf("La resta de %.2f y %.2f es: %.2f\n",e,c,ANS);
			}else{
			printf("Digite los valores a restar y pulse enter\n");
			scanf("%f",&b);
		    scanf("%f",&c);
		    ANS=b-c;
		    printf("La resta de %.2f y %.2f es: %.2f\n",b,c,ANS);
			}
			e=ANS;
		    break;
		    case 3: //printf("Digite los valores a multiplicar y pulse enter\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite el segundo numero\n");
		    	scanf("%f",&c);
		    	ANS=e*c;
		    	printf("La multiplicacion de %.2f y %.2f es: %.2f\n",e,c,ANS);
			}else{
			printf("Digite los valores a multiplicar y pulse enter\n");
			scanf("%f",&b);
		    scanf("%f",&c);
		    ANS=b*c;
		    printf("La multiplicacion de %.2f y %.2f es: %.2f\n",b,c,ANS);	
			}
			e=ANS;
		    break;
		    case 4: //printf("Digite los valores a dividir y pulse enter\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite el segundo numero\n");
		    	scanf("%f",&c);
		    	ANS=e/c;
		    	printf("La division de %.2f y %.2f es: %.2f\n",e,c,ANS);
			}else{
			printf("Digite el numerador\n");
		    scanf("%f",&b);
		    printf("Digite el divisor\n");
		    scanf("%f",&c);
		    ANS=b/c;
		    printf("La division de %.2f y %.2f es: %.2f\n",b,c,ANS);
			}
			e=ANS;
		    break;
		    case 5: //printf("Digite el numero a aplicarle porcentaje\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite el valor del porcentaje que quiere obtener del resultado anterior\n");
		    	scanf("%f",&c);
		    	ANS=(e*c)/100;
		        printf("El %.2f porciento de %.2f es: %.2f\n",c,e,ANS);	
			}else{
			printf("Digite el numero a aplicarle porcentaje\n");	
			scanf("%f",&b);
		    printf("Digite el valor del porcentaje que quiere obtener del numero\n");
		    scanf("%f",&c);
		    ANS=(b*c)/100;
		    printf("El %.2f porciento de %.2f es: %.2f\n",c,b,ANS);
			}
			e=ANS;
		    break;
		    case 6: //printf("Digite la base de la expresion\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	printf("Digite la potencia de la expresion\n");	
		    	scanf("%f",&c);
		    	ANS = pow(e,c);
		    	printf("El resultado de la potenciacion es: %.2f\n",ANS);
			}else{
			printf("Digite la base de la expresion\n");
			scanf("%f",&b);
		    printf("Digite la potencia de la expresion\n");
		    scanf("%f",&c);
		    ANS = pow(b,c);
		    printf("El resultado de la potenciacion es: %.2f\n",ANS);
			}
			e=ANS;
		    break;
		    case 7: //printf("Digite el argumento del logaritmo en base 10\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		     scanf("%i",&d);
		    if(d==14){
		    	ANS = log10(e);
		        printf("El logaritmo en base 10 de %.2f es: %.2f\n",e,ANS);
			}else{
			printf("Digite el argumento del logaritmo en base 10\n");
			scanf("%f",&b);
		    ANS = log10(b);
		    printf("El logaritmo en base 10 de %f es: %.2f\n",b,ANS);
			}
			e=ANS;
		    break;
		    case 8: //printf("Digite un numero para conocer el sin de este\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	ANS = sin(e);
		    	printf("El seno de %.2f es: %.2f\n",e,ANS);
			}else{
			printf("Digite un numero para conocer el sin de este\n");
			scanf("%f",&b);
		    ANS = sin(b);
		    printf("El seno de %.2f es: %.2f\n",b,ANS);
			}
			e=ANS;
		    break;
		    case 9: //printf("Digite un numero para conocer el coseno de este\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	ANS = cos(e);
		    	printf("El coseno de %.2f es: %.2f\n",e,ANS);
			}else{
			printf("Digite un numero para conocer el coseno de este\n");
			scanf("%f",&b);
		    ANS = cos(b);
		    printf("El coseno de %.2f es: %.2f\n",b,ANS);	
			}
			e=ANS;
		    break;
		    case 10: //printf("Digite un numero para conocer la tangente de este\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	ANS = tan(e);
		    	printf("La tangente de %.2f es: %.2f\n",e,ANS);
			}else{
			printf("Digite un numero para conocer la tangente de este\n");
			scanf("%f",&b);
		    ANS = tan(b);
		    printf("La tangente de %.2f es: %.2f\n",b,ANS);
			}
			e=ANS;
		    break;
		    case 11: //printf("Digite un numero para conocer su raiz cuadrada\n");
		    printf("si quiere utilizar el resultado anterior digite 14 si no digite 0\n");
		    scanf("%i",&d);
		    if(d==14){
		    	if(e<0){
		    		printf("No es posible calcular la raiz de un numero negativo\n");
				}else{
					ANS = sqrt(e);
					printf("La raiz de %.2f es: %.2f\n",e,ANS);
				}
			}else{
			printf("Digite un numero para conocer su raiz cuadrada\n");
			scanf("%f",&b);
		    if (b<0) {
		    	printf("No es posible calcular la raiz de un numero negativo\n");
			}else{
				 ANS = sqrt(b);
		    printf("La raiz de %.2f es: %.2f\n",b,ANS);
			}
			e=ANS;
			break;
			}
	    }
	}while(a!=13);

	
	return 0;
	
}
	
	
