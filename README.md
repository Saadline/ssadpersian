راهنمای مختصر برای افراد تازه‌کار
برای اینکه بتوانید به راحتی از این نرم‌افزار استفاده کنید، نیاز است که با توابع، پارامترها و کاراکترهای آن آشنا شوید. ابتدا با اصطلاحات اصلی آشنا شوید:

برچسب زمان (TimeStamp)

برچسب زمانی (Unix) یک عدد بر حسب ثانیه است که می‌توان آن را به عنوان شماره شناسنامه یا اثر انگشت زمان دانست. این عدد از روز 1/1/1970 میلادی، دقیقاً ساعت 00:00:00 به وقت گرینویچ (GMT) شروع به شمارش کرده است و هر یک ثانیه که می‌گذرد، یک واحد به آن اضافه می‌شود. مثلاً سایت شما برای ذخیره یک مطلب جدید، به جای ذخیره عبارت طولانی "جمعه، 22/بهمن/1389 - 16:07:53"، کافیست برچسب زمانی آن لحظه را ذخیره کند. در زمان لازم، می‌توانید با وارد کردن این عدد کوتاه، قالب‌های مختلف تاریخ و زمان را از توابع مربوطه دریافت کنید.

تابع (Function)

توابع موجود در این نرم‌افزار، در جدول مربوطه فهرست شده‌اند. توابع اطلاعاتی را از ما دریافت کرده، تغییرات لازم را اعمال کرده و خروجی را بازمی‌گردانند. مثلاً تابع gregorian_to_jalali شماره سال، ماه و روز میلادی را دریافت کرده و شماره سال، ماه و روز هجری شمسی را بازمی‌گرداند.

پارامتر (Parameter)

پارامترها به هنگام فراخوانی، آرگومان نامیده می‌شوند. هر تابع دارای پارامترهایی است که در جدول مربوطه فهرست شده‌اند. پارامترهای اجباری، پارامترهایی هستند که حتماً باید مقداری برایشان وارد شود وگرنه تابع خروجی ندارد. پارامترهای اختیاری، پارامترهایی هستند که می‌توانند وارد نشوند. در این صورت مقدار پیشفرض برای آن پارامتر استفاده می‌شود.

کاراکتر (Character)

کاراکترها همان حروف، اعداد و یا عبارات هستند که در جای پارامترها قرار می‌گیرند. هر پارامتر یک تابع می‌تواند مقادیر خاصی را بگیرد که این مقادیر همان کاراکترها هستند. مثلاً در تابع jdate پارامتر اول آن می‌تواند کاراکترهای مختلفی مثل Y برای سال کامل و y برای سال دو رقمی و s برای نمایش ثانیه را بگیرد.

استفاده‌ی ساده
اولین قدم برای استفاده از این نرم‌افزار، افزودن فایل jdf.php به پروژه است. برای این کار، از دستور include یا include_once استفاده کنید. سپس تمامی توابع موجود در فایل را در دسترس خواهید داشت و می‌توانید از آن‌ها استفاده کنید. برای درک بهتر مطالب، یک فایل PHP آزمایشی ایجاد کنید.

یک نرم‌افزار ویرایشگر PHP را باز کنید (می‌توانید از نوت‌پد ویندوز استفاده کنید). کد زیر را در نوت‌پد بنویسید و فایل را به نام zaman.php ذخیره کنید. فایل jdf.php را در کنار فایل آزمایشی قرار دهید.

- - - - - - - -


<?php
include_once('jdf.php'); // افزودن فایل نرم‌افزار
/* کدهای آزمایشی را در این جا قرار دهید */

echo $out; // نمایش خروجی
?>


به عنوان اولین آزمایش، متغیر $out را به این صورت تنظیم کنید:

$out = jdate('F'); // خروجی: بهمن


عبارتی که نمایش داده می‌شود نام ماه به حروف است. مثلاً: "بهمن" یا هر ماه دیگری که اکنون در آن قرار داریم. کاراکتر F بزرگ تعیین می‌کند که خروجی تابع jdate نام ماه به حروف باشد.

مثال‌های دیگر
برای نمایش ساعت، دقیقه و ثانیه:
$out = jdate('H:i:s'); // خروجی: 10:15:26


برای نمایش سال، ماه و روز به عدد:


$out = jdate('Y / F / j'); // خروجی: 1389 / 11 / 22



نکته‌ها
بزرگی و کوچکی حروف اهمیت دارد و می‌تواند نتیجه را تغییر دهد.
خروجی‌های مثال‌ها در زمان شما به وقت خودتان نمایش داده خواهند شد.
نتیجه‌گیری
با مطالعه آموزش‌ها و جدول‌های راهنما، با توابع و پارامترهای مختلف آشنا شوید. این توابع کاربردهای زیادی دارند و می‌توانند زمان ثبت مطالب سایت یا نظرات بازدیدکنندگان را به تاریخ هجری شمسی و به وقت تهران ذخیره کنند. فراموش نکنید که همه از صفر شروع کرده‌اند، شما هم می‌توانید.
