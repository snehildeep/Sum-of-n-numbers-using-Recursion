# Sum-of-n-numbers-using-Recursion

#include<stdio.h>
int sum(int n);



int sum(int n){

    if(n==1){
        return 1;
    }
    int sumnm1=sum(n-1);
    int sumn= sumnm1+n;
    return sumn;

}

int main(){
    int a;
    scanf("%d",&a);

    printf("%d",sum(a));
    return 0;
}

