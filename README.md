# 2D-ARRAY-IF-AN-ELEMENT-IS-ZERO-PRINTS-THE-WHOLE-ROW-AND-COLUMN-ZERO
#include <iostream>

using namespace std;

int main()
{
    int m,n,i,j,k;
    cout<<"ENTER THE SIZE OF ROWS AND COLUMNS\n";
    cin>>m>>n;
    int a[m][n],b[m][n];
    cout<<"ENTER"<<m*n<<" NUMBERS\n";
    for(i=0;i<m;i++){
       for(j=0;j<n;j++)
       {
          cin>>a[i][j];
          b[i][j]=a[i][j];
       }
    }
    
    for(i=0;i<m;i++)
        {
            for(j=0;j<n;j++)
            {
                if(a[i][j]==0)
                {
                    for(k=0;k<m;k++)
                      b[i][k]=0;
                    for(k=0;k<n;k++)
                       b[k][j]=0;
                }
            }
        }
         for(i=0;i<m;i++){
       for(j=0;j<n;j++)
       {
          cout<<b[i][j]<<" ";
       }
       cout<<endl;
    }

    return 0;
}
