----
# **PROGRAMMING FOR PROBLEM SOLVING ESC-18105**
----
![](https://nptel.ac.in/content/college_assets/college_logo/1078_logo.jpg)
----
## **NAME** - *KAJAL TIWARY*
## **ROLL NO.** - *1914146*
## **BRANCH** - *CIVIL*
----
# PROGRAMS
----

## 1. SUM OF TWO NUMBERS
```C
#include<stdio.h>
void main()
{
        int a,b;
        printf("enter the two number to be added\n");
        scanf("%d%d",&a,&b);
        printf("Sum  : %d + %d = %d \n",a,b,a+b);

}
```

----
## 2. AVERAGE OF N NUMBERS
```C
#include<stdio.h>
void main()     
{
        int n;
        float sum=0;
        printf("enter number of elements \n");

        scanf("%d",&n);
        int a[n];
        printf(" now enter %d elements\n",n);
        for(int i=1;i<=n;i++)
        {       
                scanf("%d",&a[i]);
                sum+=a[i];
        }
        float avg;
        avg = sum/n;
        printf("average of %d elements is %0.2f \n",n,avg);
}       
```

----
## 3. WEEKDAYS
```C
#include<stdio.h>
void main()
{
        int a;
        printf("enter any integer between 1 to 7\n");
        scanf("%d",&a);
        switch(a)
        {
                case 1:
                        printf("MONDAY\n");
                        break;
                case 2:
                        printf("TUESDAY\n");
                        break;
                case 3:
                        printf("WEDNESDAY\n");
                        break;
                case 4:
                        printf("THRUSDAY\n");
                        break;
                case 5:
                        printf("FRIDAY\n");
                        break;
                case 6:
                        printf("SATURDAY\n");
                        break;
                case 7:
                        printf("SUNDAY\n");
                        break;
                default :
                        printf("enter number between 1 to 7\n");
                        break;
        }
}  
```

----
## 4. EVEN ODD CHECK
```C
#include<stdio.h>
void main()
{
        int a;
        printf("enter the number\n");
        scanf("%d",&a);
        if(a%2==0)
                printf("EVEN\n");
        else
                printf("ODD\n");
}
```

----
## 5. TABLE OF ANY NUMBER
```C
#include<stdio.h>
int main()
{
        int n,i;
        printf("enter the number \n");
        scanf("%d",&n);
        printf("\t\t\tTABLE OF %d\n",n);
        printf("\t\t\t==========\n");
        for(i=1;i<11;i++)
        {
                printf("%d * %d = %d\n",n,i,n*i);
        }               
        return 0;       
}
```

----
## 6. ARMSTRONG NUMBER
```C
#include<stdio.h>
int main()
{
        int sum=0,digit;
        int n, temp;
        printf("enter any positive integer number");
        scanf("%d",&n);
        temp=n;
        while(temp>0)
        {
                digit=temp%10;
                temp/=10;
                sum=sum+digit*digit*digit;
        }
        if(n==sum)
                printf("\n %d is a armstrong number\n",n);
        else
                printf("\n %d is not a armstrong number\n",n);
}
```

----
## 7. **CALCULATOR DIAGRAM
```C**
#include<stdio.h>


void main()
{
        
        puts(" _______________ ");
        puts("|_______________|");
        puts("| 1 | 2 | 3 |   |");
        puts("|___|___|___|   |");
        puts("| 4 | 5 | 6 | + |");
        puts("|___|___|___|___|");
        puts("| 7 | 8 | 9 | - |");
        puts("|___|___|___|___|");
        puts("|     0     | * |");
        puts("|___________|___|");

}
```
----
## 8. BUBBLE SORT
```C
#include<stdio.h>
int main()
{
        int i,n,k,temp;
        printf("\n enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter %d elements of array\n",n);
        for(i=0;i<n;i++)
                scanf("%d",&a[i]);
        for(k=0;k<n-1;k++)
        {
                for(i=0;i<n-k-1;i++)
                {
                        if(a[i]>a[i+1])
                        {
                                temp=a[i];
                                a[i]=a[i+1];
                                a[i+1]=temp;
                        }
                }
        }
        printf("\n array elements after shorting\n");
        for(i=0;i<n;i++)
                printf("%d\t",a[i]);
        printf("\n");
}
```

## 9. BINARY SEARCH
```C
#include<stdio.h>
        
int check(int b[],int m,int o)
{       
        int p=-1,mid;
 int f=1,l=m;
 mid=(f+l)/2;           

while(f<=l)
 {
        mid=(f+l)/2;
        if(b[mid]==o)
        {
                p=mid;
                break;
        }
        else if(o>b[mid])
        {
                f=mid+1;
        }
        else if (o<b[mid])
        {
                l=mid-1;
        }
        
}       
                        return p;
        
}     
       
void main()
{       
        int n,num,index;
        printf("enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter the array elements in assending order\n");
        for(int i=1;i<=n;i++)
        {
                scanf("%d",&a[i]);
        }
        printf("now enter the number which you want to check\n whether it is present or not in entered array\n");
        
        scanf("%d",&num);
        index=check(a,n,num);
        if(index==-1)   
        printf("element is not found\n");
        else
        printf("element is found at the position %d \n",index);

}
```
----
## 10. FACTORIAL OF A NUMBER
```C
              
#include<stdio.h>
int main()
{       
        int n;
        printf("enter number\n");
        scanf("%d",&n);
        int p=1;
        for(int i=1;i<=n;i++)
        {
                p*=i;
        }
        printf("%d! = %d \n",n,p);
}
```
----
##  11. FIZZ-BUZZ
```C
#include<stdio.h>
int main()
{
        for(int i=1;i<=30;i++)
                {
                        if(i%15==0)
                                printf("fizzbuzz\n");
                        else if(i%5==0)
                                printf("buzz\n");
                        else if(i%3==0)
                                printf("fizz\n");
                        else {printf("%d\n",i);}
                }
        return 0;
}
```

----
## 12. SUM OF FIRST 100 NUMBERS
```C
#include<stdio.h>
int main()
{
        int sum=0,i=1;
        while(i<101)
        {
                sum =sum+i;
                i++;
        }
        printf("sum of numbers from 0 to 100 is %d\n",sum);
        return 0;
}
```

----
## 13. FIND GREATER BETWEEN TWO NUMBERS
```C
#include<stdio.h>
void main()
{       
        float a,b;
        printf("enter first number\n");
        scanf("%f",&a);
        printf("enter the second nummber\n");
        scanf("%f",&b);
        if(a>b)
                printf("%f is greater\n",a);
        else if(b>a)
                printf("%f is greater\n",b);
        else    
                printf("both numbers are equal\n");
}
```
----
## 14. GREATER AMONG THREE NUMBERS
```C
#include<stdio.h>
void main()
{
int a,b,c;
printf("enter the three numbers which you want to compare \n");
scanf("%d%d%d",&a,&b,&c);
if(a>b&&a>c)
printf("\n%d is the greatest number\n",a);
else if(b>a&&b>c)
printf("\n%d is the greatest number\n",b);
else 
printf("\n%d is the greatest number\n",c);
}
```
----
## 15. GREATEST INTEAGER FUNCTION
```C
#include<stdio.h>
int gcd(int a,int b)
{
        int c;
        c=a%b;
        if(c==0)
                return b;
        else 
                gcd(b,c);
}
int main()
{
        int m,n,c;
        scanf("%d%d",&m ,&n);
        c=gcd(m,n);
        printf("\n gcd is %d \n",c);
        return 0;
}
```
 ----
 ## 16. LEAP YEAR CHECK
 ```C
 #include<stdio.h>
int main()
{
        int a;
        printf("enter the year\n");
        scanf("%d",&a);
        if(a%4==0)
        printf("it is a leap year\n");
        else
                printf("it is not a leap year\n");
}
```
----
## 17. LINEAR SEARCH
```C
#include<stdio.h>

int check(int b[],int m,int o)
{int p=-1;
        for(int i=1;i<=m;i++)
        {
                if(b[i]==o)
                 p = i;
        }

                        return p;
        
}

void main()
{
        int n,num,index;
        printf("enter the array size\n");
        scanf("%d",&n);
        int a[n];
        printf("enter the array elements\n");
        for(int i=1;i<=n;i++)
        {
                scanf("%d",&a[i]);
        }
        printf("now enter the number which you want to check\n whether it is present or not in entered array\n");

        scanf("%d",&num);
        index=check(a,n,num);
        if(index==-1)
        printf("element is not found\n");
        else
        printf("element is found at the position %d \n",index);
}
```
----
##  18. SUM OF TWO MATRIX
```C
#include<stdio.h>       
int main()                      
{                       
        int m,n,o,p,i,j;
        printf("enter the number of rows and columns of matries \n");
        scanf("%d %d",&m,&n);
        int a[m][n] , b[m][n] , c[m][n];
        {               
                printf("enter the elements of first matrix\n");
                for(i=0;i<m;i++)
                {       
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&a[i][j]);
                        }
                }       
                printf("enter the elements of second matrix\n");
                for(i=0;i<m;i++)
                {               
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&b[i][j]);
                        }
                }
                printf("the elements of first matrix is \n");
                for(i=0;i<m;i++)
                {               
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",a[i][j]);
                        }
                        printf("\n");
                }
                   printf("the elements of second matrix is \n");
                for(i=0;i<m;i++)
                {       
                        for(j=0;j<n;j++)
                        {       
                                printf("%d ",b[i][j]);
                        }
                        printf("\n");
                }
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                {
                                        c[i][j]=a[i][j]+b[i][j];
                                
                                }
                        }
                }
                      
                printf("sum of given matrices is\n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",c[i][j]);
                        }       
                        printf("\n");
                }       
        }       
                
}               
                        
```


----
## 19. TRANSPOSE MATRIX
```C
#include<stdio.h>
int main()
{ 
        int m,n,i,j;
        printf("enter the number of rows and columns of matrix\n");
        scanf("%d%d",&m,&n);
        int a[m][n],b[m][n] ;
                printf("enter the elements of  matrix row wise\n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                scanf("%d",&a[i][j]);
                        }       
                }       
                
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                b[j][i]=a[i][j];
                        }       
                }       
                printf("transpose  of matrix is \n");
                for(i=0;i<m;i++)
                {
                        for(j=0;j<n;j++)
                        {
                                printf("%d ",b[i][j]);
                        }       
                        printf("\n");
                }       
}               
```
----
## 20. SUM OF DIGITS OF A NUMBER
```C
#include<stdio.h>
int main()
{
        int a,sum=0,c;
        printf("enter the number\n");
        scanf("%d",&a);
        while(a!=0)
        {
        c=a%10;
        sum+=c;
        a=a/10;
        }
        printf("sum of digits is %d\n",sum);
}
```
----
## 21. CHECK PALINDROME NUMBER
```C
#include<stdio.h>
int main()
{
        int sum=0,digit;
        int n, temp;
        printf("enter any positive integer number\n");
        scanf("%d",&n);
        temp=n;
        while(temp>0)
        {
                digit=temp%10;
                temp/=10;
                sum=sum*10+digit;
        }
        if(n==sum)
                printf("\n %d is a palidrome number\n",n);
        else
                printf("\n %d is not a palidrome number\n",n);
}
```
 ----
 ## 22. CALL BY VALUE
 ```C
 #include<stdio.h>
void swap(int a,int b);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(x,y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int a,int b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",a,b);
temp=a;
a=b;
b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",a,b);
}
```
----
## 23. CALL BY REFERENCE
```C
#include<stdio.h>
void swap(int *,int *);
void main()
{
int x,y;
printf("\n Enter value for x:");
scanf("%d",&x);
printf("\n Enter value for y:");
scanf("%d",&y);
printf("\n Before calling swap functin\n");
printf("\n Value of x=%d,Value of y=%d\n",x,y);
swap(&x,&y);
printf("\n After returning from swap function");
printf("\n Value of x=%d,value of y=%d\n",x,y);
}
void swap(int *a,int *b)
{
int temp;
printf("\n Inside the function \n");
printf("\n Value of a=%d,Value of b=%d before swaping\n",*a,*b);
temp=*a;
*a=*b;
*b=temp;
printf("\n Value of a=%d,Value of b=%d after swaping\n",*a,*b);
}
```
----
## 24. EMPLOYEE DETAILS USING STRUCTURE
```C
#include<stdio.h>
#include<string.h>
struct employee
{
        int code;
        char name[20];
        char department[20];
        float salary;
};
void main()
{
        struct employee e;
        printf("enter employee code\n");
        scanf("%d",&e.code);
        printf("enter employee name\n");
        scanf("%s",&e.name);
        printf("enter employee department\n");
        scanf("%s",&e.department);
        printf("enter employee salary\n");
        scanf("%f",&e.salary);
        printf("information about employee is \n");
        printf("Employee code: %d \n",e.code);
        printf("Employee name: %s \n",e.name);
        printf("Employee department: %s \n",e.department);
        printf("Employee salary: %f \n",e.salary);
}
```
----
## 25. FRACTION PRODUCT USING STRUCTURE
```C
#include<stdio.h>
struct fraction
{
        int num;
        int den;
};
void main()
{
        int rnum,rden;
        struct fraction f1,f2;
        printf("enter numerator and denominator of first fraction\n");
        scanf("%d%d",&f1.num,&f1.den);
        printf("enter numerator and denominator of second fraction\n");
        scanf("%d%d",&f2.num,&f2.den);  
        rnum=f1.num*f2.num;
        rden=f1.den*f2.den;
        printf("\nproduct is : %d/%d\n",rnum,rden);
}
```

