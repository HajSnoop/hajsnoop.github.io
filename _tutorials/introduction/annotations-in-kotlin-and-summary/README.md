---
layout: tutorial
title: "annotation ها در کاتلین و خلاصه بخش هشت"
category: introduction
permalink: /tutorials/introduction/annotations-in-kotlin-and-summary/
editlink: https://github.com/KotlinFarsi/OpenSourceTutorials-Introduction/edit/master/src/annotations-in-kotlin-and-summary/README.md
---


<div dir="rtl" markdown="1">



درواقع Annotation های کاتلین کاملا با Annotation های جاوا همسو هستن. در قسمت Advance میبینیم که چه طور Annotation های دلخواه خودمون رو درست کنیم ولی فعلا یادتون میدم که چجوری بتونین از Annotation های آماده ی جاوا استفاده کنید.

برای یادگیری این مبحث لازمه که حداقل با Junit اشنا باشین و Junit رو به پروژتون اضافه کنین

</div>

```kotlin
import org.junit.Test

class AnnotationsTest{
    @Test fun testAnnotation(){
        
    }
}
```

<div dir="rtl" markdown="1">

دقیقا به همون طریقی که Annotation هارو توی جاوا استفاده میکردیم اینجا هم با قراردادن @ میتونیم از اون ها استفاده کنیم.

همینطور که کلاس هارو میتونیستم با استفاده از as با نام دیگه صدا بزنیم اینجاهم میتونیم همین کار رو انجام بدیم

</div>

```kotlin
import org.junit.Test as Specification

class AnnotationsTest{
    @Specification fun testAnnotation(){

    }
}
```

<div dir="rtl" markdown="1">

**خلاصه بخش 8:**

1-	با SmartCasting اشنا شدیم

2-	فهمیدم که چندگانه ها در کاتلین محدود هستند، بیشتر از 3گانه باید از کلاس های دیتا استفاده بشه

3-	یادگرفتیم چگونه یک مقدار رو بشکنیم و این زمانیکه میخوایم از کلاس های دیتا یا چندگانه ها استفاده کنیم مفیده و معنی بهتری داره

4-	نیازی به Exception های چک شده در کاتلین وجود ندارند.

5-	Constant ها میتونند یا به صورت objectو یا به عنوان خصیصه های Top-Level استفاده بشن

6-	Annotation ها در کاتلین قابل دسترسی اند و همچنین Annotation های جاوا رو میشه در کاتلین استفاده کرد


</div>
