# LTIME104C
#  LOCKDRAW 
for i in range(int(input())):
    a,b,c=map(int,input().split())
    if (a==(b+c))or(b==(a+c))or(c==(a+b)):
        print("Yes")
    else:
        print("No")
        
#  SUBSTADD in c language
#include <stdio.h>

int main(void) {
	// your code goes here
	int t;
	scanf("%d",&t);
	while(t--){
	    int n,x,y;
	    scanf("%d %d %d",&n,&x,&y);
	    int a[n],b[n];
	    for(int i=0;i<n;i++){
	        scanf("%d",&a[i]);
	    }
	    for(int i=0;i<n;i++){
	        scanf("%d",&b[i]);
	    }
	    int c=1;
	    for(int i=0;i<n;i++){
	        if((b[i]-a[i]!=x)&&(b[i]-a[i])!=y){
	        c=0;
	        break;
	        }
     	}
	if(c==0)
	printf("NO\n");
	else
	printf("YES\n");}
	return 0;
}

# SUBPERM 
for i in range(int(input())):
    n,k=map(int,input().split())
    if n==1:
        print(1)
    elif k==1:
        print(-1)
    else:
        for j in range(k,n+1):
            print(j,end=" ")
        for j in range(1,k):
            print(j)
