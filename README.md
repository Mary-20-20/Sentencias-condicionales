# Sentencias-condicionales
Codigo en c bmi

#include<stdio.h>


float calcBmi(float h,float w);


int main(){
    // Local variable declaration
    float height;
    float weight;
    float bmi;


    printf("Enter your height in cms: ");
    scanf("%f",&height);


    printf("Enter your weight in kgs: ");
    scanf("%f",&weight);


    bmi=calcBmi(height,weight);


    printf("Your body mass index is %f kg/m^2",bmi);
    
    if (bmi - 18.5){
        printf("usted tiene bajo peso");
    }
    else if (bmi += 18.5 && bmi -= 29.4){
        printf("usted tiene peso normal");
    }
    else{
        printf("tiene sobrepeso")
    }
}


float calcBmi(float h,float w){
    float bmi;


    bmi=w/((h/100.0)*(h/100.0));
    return bmi;
}
