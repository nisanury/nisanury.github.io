---
layout: post
title:  "C Programlama Dilinden Sorular 1"
image: ''
date: 2018-05-19 20:23:30
tags:
- Programlama Dilleri
description: 'Programlama Dillerine giriş.'
categories:
- C
serie: başlangıç
---  
**1.Soru:**  
Amstrong sayıları bulan program;  
{% highlight c %}  
#include<conio.h>  
#include<stdio.h>  

int main(){  
	int a,b,c,kupu,sayi,k=1;  
	for(a=1;a<=9;a++){  
		for(b=0;b<=9;b++){  
			for(c=0;c<=9;c++){  
			sayi=100*a+10*b+c;  
			kupu=a*a*a+b*b*b+c*c*c;  
			if(sayi==kupu)  
			printf("%d. %d \n",k++,sayi);  
			}  
		}  
	}  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Şeklinde bir çıktı alırız;  
![](/assets/img/amst.png)  
  
**2.Soru:**  
1'den 100 kadar olan asal sayıları bulan program;
{% highlight c %}  
#include <stdio.h>   
#include<conio.h>  

int main()   
{  	 
int i,j,d;  

	for(i=2;i<=100;i++)   
{  
	d=1;  
	for (j=2;j<i;j++)   
{  	
	if (i%j==0)   
{  
	d=0;  
}}  

	if (d==1) {  
printf("%d\n",i);  
}}  
getch();  
return 0;   
}  
{% endhighlight %}  
Şeklinde bir çıktı oluşur;  
![](/assets/img/asal.png)  
  
**3.Soru:**  
Fibonacci Dizisi;
{% highlight c %}  
#include <stdio.h>  
#include <conio.h>  
 
int main(){  
    
    int birinciSayi=0, ikinciSayi=1, ucuncuSayi;  
    for(int i=1; i<=45; i++){  
    
    if (i == 1)  
        printf("%d %d ", birinciSayi, ikinciSayi);  
        
    ucuncuSayi = birinciSayi + ikinciSayi;  
    birinciSayi = ikinciSayi;  
    ikinciSayi = ucuncuSayi;  
     
    printf("%d ", ucuncuSayi); //Ekrana yazdır  
    
    if( i % 5 == 0) // her 5 sayıda bir satır aşağı iner  
        printf("\n");  
    }  
    getch();  
    return 0;  
}  
{% endhighlight %}  
Şeklinde bir çıktı oluşur;   
![](/assets/img/fibo.png)  

**4.Soru:**  
Kullanıcının girdiği sayıların kaç tanesinin negatif olduğunu bulan program;  
{% highlight c %}  
#include<conio.h>  
#include<stdio.h>  

int main()  
{  
	int sayi,sayac=0,i=1;  
	for(i=1; i<=10;i++){  
	printf("%d. sayi: ",i);  
	scanf("%d",&sayi);  
	if(sayi<0)  
	sayac++;  
}  
printf("%d tane negatif.",sayac);  
getch();  
return 0;  
}  
{% endhighlight %}  
Şeklinde b çıktı alırız;  
![](/assets/img/negatifler.png)  

**5.Soru:**  
Kullanıcının belirlediği sayı kadar girilen sayıların ortalamasını bulan program;  
{% highlight c %}  
#include<stdio.h>  
#include<conio.h>  

int main()  
{  
	int sayi,toplam=0, n, ortalama=0;  
	
	printf("kac sayinin ortalamasi bulunacak: ");  
	scanf("%d",&n);  
	
	for(int i=1; i<=n; i++)  
{  
	printf("sayi giriniz: ");  
	scanf("%d",&sayi);  
	
	toplam=toplam+sayi;  
	ortalama=toplam/n;  
}  
	printf("ortalama %d \n", ortalama);  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Şeklinde bir çıktı oluşur;  
![](/assets/img/kullaniciort.png)