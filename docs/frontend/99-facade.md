---
title: Facade Design Pattern
description: How to containerized applications with docker
---

![](./images/facade.png)

# Design Patterns

در طول زمان برنامه نویسان برای توسعه نرم افزارها با مشکلات مختلفی مواجه می‌شدند. بسیاری از این مشکلات مستقل از زبان‌های برنامه نویسی و مشابه هم بودند. بنابراین برای حل این مشکلات راه حل‌های مختلفی ارائه شد که به بهترین روش حل و رفع این مشکلات الگوهای طراحی یا Design Pattern می گویند. به عبارت دیگر مجموعه ‌‌ای از بهترین راه‌ حل‌های مشکلات متداول در فرآیند برنامه نویسی نرم ‌افزار را الگوهای طراحی می‌نامند. دیزاین پترن ها برای حل مشکلات رایج در برنامه نویسی شی گرا به وسیله برنامه نویسانی باتجربه توسعه داده شده اند.
الگوهای طراحی جزو معماری‌های نرم افزاری نیستند و فقط شیوه ای صحیح از کدنویسی شی گرا را ارائه می‌دهند. بنابراین این الگوها فقط در قلمرو کدنویسی شی گرا وارد می‌شوند و مستقل از زبان‌های برنامه نویسی هستند.

# History of patterns

الگوهای طراحی اولین بار توسط کریستوف الکساندر (Christopher Alexander) ارائه شدند. کریستوف الکساندر از الگوهای طراحی تحت عنوان راه حل هایی برای مشکلاتی یاد می‌کرد که به صورت متداول در فرآیند برنامه نویسی رخ می‌دهند. در سال 1994 گروهی به اسم Gang of Four که اعضای آن را اریک گاما، ریچارد هلم، رالف جانسون، جام ولیسایدز تشکیل می‌دادند، الگوهای طراحی را از نظر کاربرد طبقه‌ بندی کردند. گروه Gang of Four یا به اختصار GOF، این الگوها را در قالب کتابی به نام الگوهای طراحی منتشر کردند. این کتاب 23 تا از الگوهای طراحی را به سه دسته کلی تقسیم بندی کرده و به معرفی و آموزش آن‌ها پرداخته است.

گاما و همکارانش در این کتاب برای معرفی هر یک از الگوهای طراحی ساختار خاصی را در نظر گرفته اند. آن‌ها از معرفی الگوهای طراحی به صورت تصویری خودداری کرده اند. زیرا بر این اعتقاد بودند که معرفی الگوهای طراحی نیازمند ساختاری جدید و اختصاصی است. بنابراین ساختار زیر را به منظور ارائه بهتر دیزاین پترن‌ها طراحی کردند. اجزای اصلی این ساختار عبارتند از :

- نام و طبقه‌ بندی: 
نام الگو و توصیفی کوتاه از آن را بیان می‌کند.
- هدف: در این بخش به صورت مختصر توضیحاتی در مورد هدف از ارائه الگو مطرح شده است.
- نام دیگر: اگر الگوی طراحی با نام‌های دیگری شناخته شده باشد در این بخش آن‌ها معرفی می‌شوند.
- راه حل: این قسمت به سناریویی که در آن از الگوی طراحی استفاده شده‌ باشد و نحوه استفاده از کلاس‌ها و شی‌ها برای حل مشکل مد نظر می‌پردازد.
- کاربرد: در این بخش توصیف می‌شود که الگوی مورد نظر در چه شرایطی کاربرد خواهد داشت.
- ساختار: در این بخش ساختار اصلی الگوهای طراحی با استفاده از UML نمایش داده می‌ شوند.
- کلاس‌ها و اشیای مورد استفاده: مسئولیت کلاس‌ها یا اشیایی که در الگوی طراحی استفاده می‌شوند در این بخش نوشته می‌شوند.
- نحوه همکاری: چگونگی همکاری کلاس‌ها و شی‌ها در این قسمت مشخص می‌شود.
- روش پیاده‌ سازی: در این بخش مراحل پیاده سازی مطرح می‌شوند.
- کد نمونه: در این بخش مثال‌ها در قالب زبان‌های برنامه نویسی نشان داده شده اند.
- مثال‌‌های کاربردی: در این بخش مثال هایی کاربردی از الگوی طراحی ذکر می‌شوند.
- ارتباط الگوی طراحی با سایر الگوها: بخش‌ها مرتبط الگوی طراحی با سایر الگوها در این بخش مورد بررسی قرار می‌گیرد.

# Classification of patterns

الگوهای طراحی با توجه به کاربردها و اهدافی که به آن منظور ارائه شده اند، به سه دسته عمومی Creational Design Patterns، Structural Design Patterns، Behavioral Design Patterns تقسیم می‌شوند.

# Creational

این دسته شامل مکانیسم ها و دستورات مشخص برای ساخت و گسترش کلاس ها و اشیاء مختلف میشوند که میتواند منجر به کاهش کد و قابل استفاده شدن کد ما کمک کند.

متداول‌ترین دیزاین پترن‌های سازنده عبارتند از :

- Singleton
- Factory Method
- Prototype
- Abstract Factory
- Builder
- Object Pool

برای آشنایی با این دسته از الگو های طراحی میتوانید به این لینک مراجعه کنید

-   [Creational Design Patterns ](https://refactoring.guru/design-patterns/creational-patterns)

# Structural

الگوهای structural به منظور مدیریت ارتباط بین کلاس ها و اشیاء مختلف میشوند
در واقع این الگوها دستور العملی برای گرد هم آوردن کلاس های مختلف را ارائه میکنند که با استفاده
آن ها میتوان کلاس های مختلف را در یک مقیاس برزگتر در کنار هم مدیریت کرد.

این الگوهای طراحی عبارتند از :

- Adapter 
- Decorator
- Facade
- Bridge
- Composite
- Flyweight
- Proxy

برای آشنایی با این دسته از الگو های طراحی میتوانید به این لینک مراجعه کنید

-   [Structural Design Patterns ](https://refactoring.guru/design-patterns/structural-patterns)

# Behavioral

آخرین دسته از الگوهای طراحی به رفتار و مسئولیت های هر کلاس می پردازد و مشخص میکند چگونه باید مسئولیت ها تقسیم شوند و وظایف هر کلاس چیست و وظایف چگونه باید مدیریت شود.

این الگوهای طراحی عبارتند از:

- Chain of responsibility
- Strategy
- Iterator
- Command
- Mediator
- Memento
- Observer
- State
- Template Method
- Visitor

برای آشنایی با این دسته از الگو های طراحی میتوانید به این لینک مراجعه کنید

-   [Behavioral Design Patterns ](https://refactoring.guru/design-patterns/behavioral-patterns)


# Why should We learn patterns?

می توان با این دیدگاه به دیزاین پترن‌ها نگاه کرد که استفاده از آن‌ها در حقیقت، بهره مندی از تجارب و تخصص بهترین برنامه نویسان شی گرا در فرآیند کدنویسی است. برخی بر این باور هستند که مشکلاتی مانند استفاده زیاد از کلاس ها، طراحی ضعیف و… جزو مشکلات بنیادی برنامه نویسی شی گرا است. دیزاین پترن‌ها با شناخت صحیح اصول برنامه نویسی شی گرا مزایای زیادی را در اختیار برنامه نویسان قرار می‌دهند. از جمله مهمترین مزایای استفاده از آن‌ها می‌توان به موراد زیر اشاره کرد:

- افزایش مقیاس پذیری (scalability)
- افزایش قابلیت توسعه پذیری (expandability)
- افزایش انعطاف پذیری (flexibility)
- افزایش سرعت توسعه نرم افزارها
- کاهش خطاها و مشکلات
- کاهش میزان کدنویسی

در این مطلب به الگوی طراحی Facade میپردازیم و نحوه پیاده سازی آن در react را بیان میکنیم.

# Facade Design Pattern

فساد (facade) یک الگوی طراحی structural است. این الگوی طراحی نقش یک رابط را بین یک کلاس پیچیده و یک کلاس با سطح کد بالاتر را ایفا میکند.
به نحوی که ارتباط این دو کلاس از طریق فساد ایجاد میشود. به مثال زیر توجه کنید:
زمانی که شما به رستورانی میروید از طریق پیشخوان فقط سفارش خود را ثبت میکنید و تمام دستورات
لازم توسط مسئول پیش خوان به باقی بخش ها داده میشود و شما دیگر نیاز با انجام کاری ندارید.
![](./images/facadeclass.png)

تمرکز ما در این مطلب به پیاده سازی این الگوی طراحی در React است معمولا الگوی طراحی facade با استفاده از Custom Hooks در ری اکت پیاده سازی میشود .
به نمونه کد زیر توجه کنید

```jsx
import React, {useEffect, useRef, useState} from 'react';
export default function BigSlider({mainbody, imgData}) {
    const Values = useRef({
        //needed values
    });
    const items = useRef(null);
    const [left, setLeft] = useState(0);
    const [index, setIndex] = useState(0);
    useEffect(() => {
        // necessary logic
    }, []);

    function HandleEventmove(event) {
        // Handle Event over
    }
    function getPosition(event) {
        // return the event position
    }
    function HandleEventDown(e) {
        // Handle Event down
    }
    function HandleEventUp(e) {
        // Handle Event Up
    }
    function shifttheAnimation(dir) {
        // set the animation for transmition
    }

    function HandleTransitionEnd(e) {
        // remove animation
    }
    return (
        <div
            id="bigslider"
            className=" ltr big-slider w-[100%] h-[300px] flex mb-[65px] vsmmobile:mb-0 vsmmobile:h-[40%]"
        >
            <div className="overflow-hidden relative h-[100%] my-[20px]">
                <div
                    onMouseMove={HandleEventmove}
                    onTouchMove={HandleEventmove}
                    onMouseUp={HandleEventUp}
                    onTouchEnd={HandleEventUp}
                    onTouchStart={HandleEventDown}
                    onMouseDown={HandleEventDown}
                    onTransitionEnd={HandleTransitionEnd}
                    ref={items}
                    className={`items w-[300%] h-[100%] ${
                        Values.current.animation ? 'transition-[left] ease-out duration-200' : ''
                    } relative top-0 flex gap-3 vsmmobile:gap-[2rem] vsmmobile:h-[85%]`}
                    style={{left: `${left}px`}}
                >
                    <div className="bigslide cursor-pointer float-left justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index - 1 + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                    <div className="bigslide  cursor-pointer float-left  justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                    <div className="bigslide cursor-pointer float-left justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index + 1 + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                </div>
            </div>
        </div>
    );
}
```

این کد به منظور ساخت یک اسلایدر در ری اکت ساخته شده است که تمام محاسبات در کد سطح بالا در معرض نمایش گذاشته شده است برای بهبود این وضعیت از فساد استفاده میکنیم و یک هوک کاستوم میسازیم و کد را به این شکل تغییر میدهیم

# UseBigSlider hook

```jsx
import React, {useEffect, useState, useRef} from 'react';
export default function useBigSlier(mainbody, imgData) {
    const [left, setLeft] = useState(0);
    const [index, setIndex] = useState(0);
    const Values = useRef({
        //needed values
    });
    const items = useRef(null);
    const [left, setLeft] = useState(0);
    const [index, setIndex] = useState(0);
    useEffect(() => {
        // necessary logic
    }, []);

    function HandleEventmove(event) {
        // Handle Event over
    }
    function getPosition(event) {
        // return the event position
    }
    function HandleEventDown(e) {
        // Handle Event down
    }
    function HandleEventUp(e) {
        // Handle Event Up
    }
    function shifttheAnimation(dir) {
        // set the animation for transmition
    }

    function HandleTransitionEnd(e) {
        // remove animation
    }

    return [HandleEventmove, Values, HandleTransitionEnd, HandleEventUp, HandleEventDown, index, left];
}
```

# BigSlider Component

```jsx
import React, {useEffect} from 'react';
import useBigSlier from '../../utility/useBigSlier';
export default function BigSlider({mainbody, imgData}) {
const [HandleEventmove, Values, HandleTransitionEnd, HandleEventUp, HandleEventDown, index,left]= useBigSlier( mainbody,imgData);
    return (
        <div
            id="bigslider"
            className=" ltr big-slider w-[100%] h-[300px] flex mb-[65px] vsmmobile:mb-0 vsmmobile:h-[40%]"
        >
            <div className="overflow-hidden relative h-[100%] my-[20px]">
                <div
                    onMouseMove={HandleEventmove}
                    onTouchMove={HandleEventmove}
                    onMouseUp={HandleEventUp}
                    onTouchEnd={HandleEventUp}
                    onTouchStart={HandleEventDown}
                    onMouseDown={HandleEventDown}
                    onTransitionEnd={HandleTransitionEnd}
                    className={`items w-[300%] h-[100%] ${
                        Values.current.animation ? 'transition-[left] ease-out duration-200' : ''
                    } relative top-0 flex gap-3 vsmmobile:gap-[2rem] vsmmobile:h-[85%]`}
                    style={{left: `${left}px`}}
                >
                    <div className="bigslide cursor-pointer float-left justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index - 1 + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                    <div className="bigslide  cursor-pointer float-left  justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                    <div className="bigslide cursor-pointer float-left justify-center transition-all duration-100 relative">
                        <img
                            className="bigcardimages  bg-skeleton"
                            src={imgData[(index + 1 + imgData.length) % imgData.length]}
                            alt=""
                        />
                    </div>
                </div>
            </div>
        </div>
    );
}
```

همانطور که مشاهده میکنید کد تغییر یافته به صورت منظم تر و ساده تر از کد اولی است که قابلیت بهبود بیشتری هم دارد.
برای آشنایی بیشتر با الگوی طراحی فساد میتوانید به لینک زیر مراجعه کنید
- [Facade](https://refactoring.guru/design-patterns/facade)