# lucky-car-number

#include <iostream>

#include <iomanip>

#include <conio.h>

#include <stdlib.h>

#include <stdio.h>

using namespace std;

 

int main()

{

    int val,n,cnt,sum=0,a;

    cout<<"Enter a number"<<endl;

    cin>>n;

    cnt=0;

    val=n;

    if(n<0)

    {

        cout<<"Number is not a valid one"<<endl;

        exit(0);

    }

    while(n>0)

    {

        a=n%10;

        cnt++;

        n=n/10;

    }

    if(cnt!=4)

    {

        cout<<"Number is not valid"<<endl;

        exit(0);

    }

     while(val!=0)

    {

        sum=sum+(val%10);

        val=val/10;

    }

    if(sum%3==0||sum%5==0||sum%7==0)

    {

        cout<<"It is a lucky car number"<<endl;

    }

    else

    {

        cout<<"It is not a lucky car number"<<endl;

    }

    getch();

    return 0;

}

 

