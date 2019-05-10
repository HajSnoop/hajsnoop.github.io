---
layout: tutorial
title: "تابع با پرامترهای نامحدود و خلاصه بخش چهارم"
category: introduction
permalink: /tutorials/introduction/function-with-unlimited-parameters-in-kotlin-and-summary
---


<div dir="rtl" markdown="1">



اخرین بخشی که میخوایم در قسمت توابع به اون نگاه کنیم، پاس دادن تعداد نامشخص پارامتر های ورودی به تابعه. به عنوان مثال من میخوام تابعی رو تعریف کنم که قبل از این که از اون استفاده کنم، تعداد نامحدودی پارامتر ورودی قبول کنه.

</div>

```kotlin
fun printStrings(vararg strings:String){
    for(string in strings){
        println(string)
    }
}
```

<div dir="rtl" markdown="1">

تابع بالا رو نگاه کنین، با استفاده از کلید واژه vararg این مفهوم رو به کامپایلر میدم که من میخوام تابعی رو استفاده کنم که تعداد ورودی هاش مشخص نیست ولی همه انها از جنس رشته هستند.

حالا من میتونم از این تابع استفاده کنم

</div>

```kotlin
printStrings("1")
printStrings("1","2")
printStrings("1","2","3")
```

<div dir="rtl" markdown="1">

و هر چه قدر که ورودی دلم بخواد به تابع پاس بدم.

فقط یک نکته اینجا هست، اگر من بخوام این vararg رو به یک تابع دیگه پاس بدم چه طور باید عمل کنم

</div>

```kotlin
fun printStrings(vararg strings:String){
    realyPrintStirngs(*strings)
}

fun realyPrintStirngs(vararg strings: String) {
    for (string in strings) {
        println(string)
    }
}
```

<div dir="rtl" markdown="1">

واقعیتش راه حل خیلی ساده است، باید یک تابع دیگه بسازیم که vararg بگیره ولی خود پارامتر vararg رو مستقیم به تابع پاس ندیم.مثلا در اینجا string رو مستقیم پاس ندیم بلکه با استفاده از "*" قبل نام پارامتر اونو پاس بدیم!

**خلاصه بخش 4**

1-	توابع با استفاده از کلیدواژه fun ساخته میشوند

2-	به صورت پیشفرص یک تابع تایپ Unit رو به عنوان پارامتر بازگشتی برمیگردونه

3-	توی توابع به ما اجازه داده شده تا از

-	پرامتر های پیشفرص داشته باشیم

-	از پارامتر های نام دهی شده استفاده کنیم

-	و بی شمار ورودی برای یک تابعمون درنظر بگیریم


