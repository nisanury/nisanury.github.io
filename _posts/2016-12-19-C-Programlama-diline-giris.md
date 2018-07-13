---
layout: post
title:  "C Programlama Diline Giriş"
image: ''
date: 2018-05-19 10:25:30
tags:
- Programlama Dilleri
description: 'Programlama Dillerine giriş.'
categories:
- C
serie: başlangıç
---  
  
    
Herhangi bir programlama dilini en iyi şekilde kavrayabilmek için öğrenmemiz gereken iki önemli adım vardır.  
Bunlardan ilki önceki yazılarda öğrendiğimiz *algoritmik düşünce*yi kafamızda iyi oturtmak ve 
hayata geçirebilmek; ikincisi ise seçtiğimiz programlama dilinin komutlarını iyi bir şekilde öğrenmek.  
  
    
Bizim ilk kavrayacağımız programlama dilimiz **C** olacak. Birkaç adım ile *C* diline olan giriş kısmımızı
tamamlamış olacağız.  
  
    

**1.Adım:**
*Temel giriş- çıkış fonksiyonları*  
C dilinde klavyeden bir değer okumak için *scanf();* fonksiyonunu kullanırız. Ekrana herhangi bir şey yazdırmak
içinde *printf();* fonksiyonu bize yardımcı olur.  
Örneğin;
{% highlight c %}
#include<stdio.h>
    int main()  
    {
        printf("Merhaba!");
    
    return 0;
    }
{% endhighlight %}  
Bu kodumuzun derlendikten sonra oluşan çıktısı Merhaba! şeklinde ekranımıza gelecektir.  
#include<stdio.h>, 
C dilinde bir kütüphaneyi temsil eder ve #include<stdio.h> yazarak programa standart 
giriş-çıkış kütüphanesini eklemiş oluruz.  
main(), ana fonksiyonu ifade eder.  

**2.Adım:**
*Kontrol Yapıları*  
**2.1 if-else Yapısı**
Bir şart durumunu ifade eder.
{% highlight c %}  
if(şart)  
    {
    //Doğru ise burası çalışır.
    }
else  
{
    //Yanlış ise burası çalışır.
}
{% endhighlight  %}  
  
![](/assets/img/operatorler.png)

**2.2 switch case Yapısı**  
{% highlight c %} 
switch(değişken)  
{  
    case değer1:
    //değişken=değer1 ise çalışır.  
    break;  
      
    case değer2:
      //değişken=değer2 ise çalışır.  
      break;  
        
    case değer3:
    //değişken=değer3 ise çalışır.  
    break;  
      
    default:  
    //Yukarıdaki değerlerden hiçbiri değilse çalışır.   
    }  
    {% endhighlight  %}  
      
**3.Adım:** *Döngüler*  
**3.1 For Yapısı:**  
{% highlight c %}  
    for(başlangıç; koşul; artım)  
{  
    ...  
    döngüdeki deyimler;  
    ...  
}  
{% endhighlight  %}  
  
**3.2 While Yapısı:**  
{% highlight c %}  
    While(koşul)  
    {  
        ...  
        döngüdeki deyimler;  
        ...  
    }  
 {% endhighlight  %}  

**3.3 Do...While Yapısı:**  
    {% highlight c %}  
    do{  
        deyimler;  
        ...  
    }  
    While(koşul);  
    {% endhighlight  %}  
*Bu yazımda C programlama dili ile ilgili genel hatlarıyla bilinmesi gereken noktaları paylaştım.*
*Giriş yazımın sonuna geldim. İleriki birkaç yazımda aşama aşama sorular çözeceğim. Büyük bir kısmı sınava*
*yönelik paylaşımlar olacaktır.*


      






