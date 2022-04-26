#include<stdio.h>
#include<math.h>
int Enter(char r){
    int number = 0;
    while (r >= '0' && r <= '1'){
        number = number*10+r - '0';
        r = getchar();
    }
        return number;
}
int Perevod(int number){
    int i = 0;
    int rez = 0;
    while (number != 0){
        rez += number%2*pow(2, i);
        number /= 10;
        i++;
    }
    return rez;
}
int main(){
    int number, rez;
    char r;
    int i = 0;
    printf("Enter binary numbers through space: \n");
    while ((r = getchar()) != '\n'){
        number = Enter(r);
        rez = Perevod(number);
        printf("Binary number %d: % 15d Decimal number: %d\n", i, number, rez );
    }
    return 0;
}
