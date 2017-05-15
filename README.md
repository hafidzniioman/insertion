//insertion sort
#include<stdio.h>
#include<iostream>
using namespace std;

main()
{
  int elemen, a[50],b, j, temp;

	cout <<"masukkan elemen : ";
	cin >>elemen;

	for (int i = 0; i < elemen; ++i)
	{
		cout <<"data ke- "<<i+1;
		cin >>a[i];
	}
	for (int i = 1; i < elemen; i++)
	{
		j=1;
		while(j>0 && a[j] < a[j-1])
		//for (j=i; j>=1; j--)
		{
			//if (a[j]<a[j-1])
			{
				temp = a[j];
				a[j] = a[j-1];
				a[j-1] = temp;
			}
			//else
				break;
		}
	}
	cout <<"array yang sudah disortir"<<endl;
	for (int k = 0; k < elemen; ++k)
	{
		cout <<a[k]<<" ";
	}
	return 0;
}
