#include<stdio.h>
int main(){
int i,j,n,temp;
int array[]={2,3,5,6,7,8,9,3,1,10};

for(i=0; i<n; i++){
    for(j=0;j<n-1;j++){
        if(array[j]>array[j+1]){
            temp=array[j];
            array[j]=array[j+1];
            array[j+1]=temp;
        }
    }
}



printf("Output the element \n");
for(i=0; i<n; i++){
    printf("%d\t",array[i]);
}

return 0;
}
