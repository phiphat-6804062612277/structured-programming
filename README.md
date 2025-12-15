# structured-programming
#include <stdio.h>
int main(){
    int h,m,s,im;
    scanf("%d:%d:%d",&h,&m,&s);
    printf("hour:%d\nminute:%d\nsecond:%d",h,m,s);
    printf("\nNext minutes:");
    scanf("%d",&im);
    if (im > 120){
        printf("error");
        return 0;
    }
    int cami = m + im;
    if (cami >= 120){
        h = h + 2;
        cami = cami - 120;
    }
    else if (cami > 59 && cami < 120){
        h = h + 1 ;
        cami = cami - 60 ;
    }
    if (h > 23){
        h = h - 24 ;
    }
    printf("\nhour:%d\nminute:%d\nsecond:%d",h,cami,s);
    return 0;
}
