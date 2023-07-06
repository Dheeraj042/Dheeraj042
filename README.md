- 👋 Hi, I’m @Dheeraj042
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
#include<iostream.h>
#include<stdio.h>
#include<conio.h>
int main()
{

    int n;
    cout<<"Enter the size of array: "; cin>>n;
    int a[10];

    cout<<"\nEnter the elements: ";
    for (int i=0; i<n; i++) cin>>a[i];
    for (int i=0; i<n; i++)
    {
         for (int j=i+1; j<n; j++) { if(a[i]>a[j])
              {
                  int temp = a[i];
                  a[i] = a[j];
                  a[j] = temp;
                  }
                  }
                  }

cout<<"\n Sorted Array in ascending order: ";

for (int i=0; i<n; i++)
cout<<a[i]<<" ";

cout<<"\n sorted array in descending order: ";

for(int i=n-1; i>=0; i--)
cout<<a[i]<<" ";
getch();
return 0;
}


