# Movie-Tickets
#include <stdio.h>

void main()
{
    int i,j,n,x,y,seats;
    printf("For club press 1, For executive press 2 ");
    scanf("%d",&seats);
    if (seats==2)
    {
    int arr[12][12]={{1,2,3},{4,5,6},{7,8,9}};
    
    for (i=0;i<=2;i++)
    {
        for (j=0;j<=2;j++)
        {
            printf("%d\t",arr[i][j]);
        }
        printf("\n");
    }
    
    printf("Enter the number of seats to take (each Rs.180)\n");
    scanf("%d",&y);
    for (x=1;x<=y;x++)
    {
        printf("Enter seat no. ");
        scanf("%d",&n);
    for (i=0;i<=2;i++)
    {
        for (j=0;j<=2;j++)
        {
            if (n==arr[i][j])
            {
                arr[i][j]=0;
            }
        }
    }
    }
    for (i=0;i<=2;i++)
    {
        for (j=0;j<=2;j++)
        {
            printf("%d\t",arr[i][j]);
        }
        printf("\n");
    }
    int price=180*y;
    printf("Total amount to pay Rs.%d",price);
    }
    
    
    
    else if(seats==1)
    {
        int newarr[12][12]={{1,2,3,4},{5,6,7,8},{9,10,11,12}};
        for (i=0;i<3;i++)
        {
            for (j=0;j<4;j++)
            {
                printf("%d ",newarr[i][j]);
            }printf("\n");
        }
        printf("Enter the number of seats to take (each Rs.250)\n");
        scanf("%d",&y);
        for (x=1;x<=y;x++)
        {
            printf("Enter seat no. ");
            scanf("%d",&n);
            for (i=0;i<3;i++)
            {
                for (j=0;j<4;j++)
                {
                    if (n==newarr[i][j])
                    {
                        newarr[i][j]=0;
                        
                    }
                    
                }
                
            }
            
        }
        for (i=0;i<3;i++)
        {
            for (j=0;j<4;j++)
            {
                printf("%d\t",newarr[i][j]);
                
            }
            printf("\n");
            
        }
        int price=250*y;
        printf("Total amount to pay Rs.%d",price);
        
    }
        
    
    
    }
