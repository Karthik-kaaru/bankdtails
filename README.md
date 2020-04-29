# bankdtails
To describe the details of a bank using structure
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
struct employee
{
    int empno;
    char empname[30];
    char deptname[30];
    float salary;
};
#define N 20
int main()
{
    struct employee emp[N];
    int i;
    printf("Enter the details of the employee\n");
    for(i=0;i<N;i++)
    {
        printf("Employee number:\n");
        scanf("%d",&emp[i].empno);
        printf("Employee name:\n");    
        scanf("%s",&emp[i].empname );
        printf("Employee department name:\n");                                           
        scanf("%s",&emp[i]. deptname);
    printf("Salary:\n");        scanf("%f",&emp[i].salary);
     }
    for(i=0;i<N;i++)
    {
    printf("\nEntered detail are\n");
    printf("Employee number: %d\n",emp[i].empno);
    printf("Employee name: %s\n",emp[i].empname);
    printf("Deparment: %s\n",emp[i].deptname);
    printf("Salary: %f\n",emp[i].salary);
    
}
}
