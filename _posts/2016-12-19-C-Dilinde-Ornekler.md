---
layout: post
title:  "C Programlama Dilinden Örnekler"
image: ''
date: 2018-07-19 15:23:30
tags:
- Programlama Dilleri
description: 'Programlama Dillerine giriş.'
categories:
- C
serie: başlangıç
---  
**1.Örnek:**  
4 işlemi bir arada göreceğimiz bir program yazalım;  
{% highlight c %}  
#include<conio.h>  
#include<stdio.h>  

int main()  
{  
	int sayi1, sayi2;  

	printf("Bir tam sayi giriniz: ");  
	scanf("%d", &sayi1);  

	printf("Bir tam sayi giriniz: ");  
	scanf("%d", &sayi2);  

	int sonuc=sayi1+sayi2;  
	int sonuc1=sayi1-sayi2;  
	int sonuc2=sayi1*sayi2;  
	int sonuc3=sayi1/sayi2;  

printf("Sonuc Toplam=%d\n Sonuc Fark=%d\nSonuc Carpim=%d\nSonuc Bolum=%d\n",sonuc,sonuc1,sonuc2,sonuc3);  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Şeklinde programımız tamamlanıyor.  
![](/assets/img/islem.png)
 İnt tipindeki değişkenler bize tam sayı değeri döndürür. İnt yerine double yazarsak sonuçlarımızı küsüratlı
 bir şekilde de elde edebiliriz.  
   
**2.Örnek:**  
Kullanıcı tarafından girilen 2 sayının karşılaştırılması;  
{% highlight c %}  
#include<stdio.h>  
#include<conio.h>  
int main()  
{  
	int sayi;  
	int sayi2;  
	
	printf("Bir sayi giriniz: ");  
	scanf("%d", &sayi);  
	printf("Bir sayi giriniz: ");  
	scanf("%d", &sayi2);  

	if(sayi<sayi2)  
	{  
		printf("2.sayi 1.sayidan buyuk.");  
	}  
	else if(sayi==sayi2)  
	{  
		printf("sayilar esit.");  
	}  
	else  
	{  
		printf("1.sayi 2.sayidan buyuk.");  
	}  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Şeklinde programımız tamamlanıyor.  
![](/assets/img/buyuksay.png)  
  
**3.Örnek:**  
Kullanıcı tarafından girilen vize ve final notlarına göre harf notu bulan program;  
{% highlight c %}  
#include<stdio.h>  
#include<conio.h>  
int main()  
{  
	float vize, final, ortalama;  

	printf("Vize notunuzu giriniz: ");  
	scanf("%f",&vize);  

	printf("final notunuzu giriniz: ");
	scanf("%f",&final);  

	ortalama=vize*0.4+final*0.6;  

	    if(ortalama>=90)  
	{  
		printf("AA");  
	}  
	    else if(ortalama>=85 && ortalama<90)  
	{  
		printf("BA");  
	}  
	    else if(ortalama>=75 && ortalama<=84)  
	{  
	    printf("BB");  
	}  
	    else if(ortalama>=70 && ortalama<=74)  
	{  
		printf("CB");  
	}  
        else if(ortalama>=60 && ortalama<=69)  
	{  
		printf("CC");  
	}  
		else if(ortalama>=55 && ortalama<=59)  
	{  
		printf("DC");  
	}  
		else if(ortalama>=50 && ortalama<=54)  
	{  
		printf("DD");  
	}  
		else if(ortalama>=0 && ortalama<=49)  
	{  
		printf("FF");  
	}  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Çıktımız ise şu şekildedir;  
![](/assets/img/harf.png)  
  
**4.Örnek:**  
Switch yapısı ile gün bulan program;  
{% highlight c %}  
#include<stdio.h>  
#include<conio.h>  
int main()  
{  
	int gun;  
	printf("Bir sayi giriniz: ");  
	scanf("%d" , &gun);  
	if(gun>=8)  
	{  
		printf("Bir sayi giriniz: ");  
		scanf("%d", &gun);  
	}  
	switch(gun)  
	{  
		case 1:  
			printf("pazartesi"); break;  
		case 2:  
			printf("sali"); break;    
		case 3:  
			printf("carsamba"); break;  
		case 4:  
			printf("persembe"); break;  
		case 5:  
			printf("cuma"); break;  
		case 6:  
        printf("cumartesi"); break;  
		case 7:  
			printf("pazar"); break;  
	}  
	getch();  
	return 0;  
}  
{% endhighlight %}  
Çıktımız ise şu şekildedir;  
  ![](/assets/img/sgunler.png)  
    
**5.Örnek:**  
Sıfır girilene kadar, girilen sayıların toplamını bulan program;  
{% highlight c %}  
#include<conio.h>  
#include<stdio.h>  

int main()  
{  
	int sayi,i,toplam=0;  
	do{  
	printf("sayi giriniz: ");  
	scanf("%d",&sayi);  

	toplam=toplam+sayi;  
		}  
        while(sayi!=0);  
    printf("sayılarin toplami=%d",toplam);  
		getch();  
		return 0;  
}  
{% endhighlight %}
Çıktımız ise şu şekildedir;
  ![](/assets/img/sifir.png)  
    
*Önümüzdeki sorular giriş düzeyine yönelik olacaktır.*

