# P-C
//permutation and combination code using factorial formula in c lang.
// Online C compiler to run C program online
#include <stdio.h>
#include<math.h>
int fact(int n){
    int f=1;
    for(int i=1; i<=n ; i++){
        f *= i;
    }
    return f;
}
int ncr(int n,int r){
    return fact (n)/(fact(r)*fact(n-r));//colon 
}
int main(){
    int n;
    printf("enter n:");
    scanf("%d" , &n);
    int r;
    printf("enter r:");
    scanf("%d", &r);
    int ans=ncr(n,r);
    printf("%d" , ans);
}
//entter n=5
//enter r=2
//10
  
