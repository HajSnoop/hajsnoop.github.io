---
layout: tutorial
title: "خلاصه بخش دوم"
category: introduction
permalink: /tutorials/introduction/conventions-used-with-kotlin-and-summary/
editlink: https://github.com/KotlinFarsi/OpenSourceTutorials-Introduction/edit/master/src/conventions-used-with-kotlin-and-summary/README.md
---


<div dir="rtl" markdown="1">



خب ما توی این دوره قراره که کلی کد کاتلین بزنیم، بنابر این بهتره که با یک سری قرارداد های اون آشنا بشیم. کاتلین تمرکز اصلیش روی Java بوده بنابراین ما همون قرارداد های جاوا رو دنبال میکنیم بنابراین اگر با قرارداد های جاوا آشنا نیستید بهتره که همین الان با هم یک مروری بکنیم. ما از LowerCamelCase ها برای نامگذاری استفاده می کنیم، این به این معنیه :

</div>

```kotlin
var HelloWorld // eshtebah
var helloWorld // dorost
```

<div dir="rtl" markdown="1">

تایپ ها(Types) رو با حروف درشت مینویسیم، متد ها و خاصیت هارو با lower camelcase مینویسیم ، نقطه ویزگول ها اختیاری هستند و تنها یک جا ازشون استفاده میشه( بعدا راجع بهش صحبت میکنیم) ، پکیج ها برعکس نوشته میشوند یعنی به جای introduction.kotlinfarsi.com مینویسیم com.kotlinfarsi.introduction  

شما میتونید چندی کلاس در یک فایل داشته باشید و همچنین پکیج ها نیاز ندارند که دقیقا هم نام فولدر ها باشند  هرچند که این پیشنهاد میشوند.

## خلاصه این بخش:

1-	کاتلین زبونیه که Java و هم JavaScript رو هم پوشش میده ( البته روی ورژنی از کاتلین داره کار میشه به نام Kotlin Native که اون دیگه اوج برنامه نویسیه و یک دوره مجزا نیاز داره تا بشه توضیح بدیم، این بخش درحال توسعه است)

2-	کاتلین بایت کد هایی رو درست میکنه که با JVM قابل اجرا هستش.

3-	کاملا با جاوا همزیسته، هم میتونید در جاوا از کلاس ها و توابع کاتلین استفاده کنید و هم برعکس داخل کاتلین از جاوا.
