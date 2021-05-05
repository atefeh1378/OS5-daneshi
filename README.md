# OS5-daneshi

به نام خدا

تمرینات سری ۵ آزمایشگاه سیستم عامل

عاطفه دانشی کامیاب ۹۷۴۴۰۳۰۳
 
 سوال ۱) گیت را کانفیگ نمایید تا برای هربار پوش کردن نیازی به وارد کردن یوزرنیم و پسورد نباشد.
 
 با استفاده از دستورات زیر دیگر نیازی به وارد کردن دوباره اطلاعات کاربری نخواهد بود.
 
 git config user.name "your name"
 
 در اینجا بجای یورنیم نام کاربری خود در گیت هاب را وارد می کنیم.
 
 git config user.password "your password"
 
 در اینجا بجای یورپسورد رمز کاربری خود در گیت هاب را وارد می کنیم.
 
 در آخر :
 
 git config --global credential.helper store
 git pull
 
سوال ۲) مفاهیم زیر را توضیح دهید.

.gitignore :

این فایل مشخص می کند که کدام فایل ها و فولدرهای پروژه را گیت باید صرف نظر کند و تغییرات آنها را نادیده بگیرد و آن ها را دنبال نکند.

.git :

این پوشه تمامی فایل های پروژه ما را دنبال می کند و حواسش به تغییرات آنها هست .داخل این پوشه اطلاعات مربوط به گیت نگهداری میشوند و اگر آن را پاک کنیم سابقه پروژه ما پاک می شود.

git pull :

دریافت آخرین تغییرات از سرور و مرج کردن آنها با این دستور انجام می شود.

branch :

شاخه یا برنچ یک کپی از پروژه اصلی هستند زمانی که ما میخوایم ویژگی های جدیدی را در برنامه خودمون ایجاد کنیم بهتر است که از این شاخه ها استفاده کنیم تا اگر برناممون به مشکلی خورد بتوانیم بدون هیچ زحمتی به نسخه قبلی برنامه خودمون برگردیم. 
شاخه پیش فرض هر ریپازیتوری مستر نام دارد بنابراین هر ریپازیتوری حداقل یک شاخه به نام مستر دارد .

سوال ۳) در کلاس یک ریپازیتوری جدید در گیت هاب ایجاد کردیم سپس آن را  کلون کردیم و سپس فایل های خود را در آن دایرکتوری خالی قرار دادیم .
حالا فرض کنید می خواهیم برعکس فرایند بالا را انجام دهیم یعنی ابتدا یک دایرکتوری خالی روی سیستم خود ایجاد کنیم سپس فایل های خود را در آن قرار دهیم و در انتها آن را به گیت هاب متصل کنیم . با استفاده از چه دستوراتی می توان این فرایند را انجام داد؟

ابتدا در مسیر مورد نظر خود می رویم و با دستور mkdir دایرکتوری خالی ایجاد می کنیم و به مسیر پوشه ای که ساختیم می رویم . 
برای مثال : ابتدا با دستور سی دی وارد مسیر داکیومنتس می شویم و پوشه ای در مسیر آن ایجاد می کنیم حال دوباره با همان دستور سی دی وارد مسیر پوشه خود می شویم .


cd Documents/
mkdir ati
cd ati


با اجرای دستور زیر به سیستم اعلام می کنیم که این فولدری که ایجاد کردیم یک ریپازیتوری یا مخزن گیت است .

git init

 دستور زیر تمامی فایل های مورد نظر ما را به وب سایت اضافه می کند.
 
 git add --all
 
 وقتی که فایل های خود را با دستور بالا اضافه کردیم کارمان برای اپلود اماده اس و پیغامی برای آن می نویسیم .
 
 git commit -m "some-message"
 
 
 حال به سایت گیت هاب خود رفته و در آنجا یک ریپازیتوری جدید به نام همان مخزنی که در ابتدا ایجاد کردیم می سازیم (در قسمت بالا من مخزنی با نام عاطی ساختم پس ریپازیتوری جدیدی که در وبسایت ساختم با همان نام است.)
 
 با استفاده از دستور زیر به مخزن در گیت هاب وصل می شویم .
 
 
 git remote add origin address.
 
 
 در اینجا ادرس مخزنی که ایجاد کردیم را بجای آدرس در جمله بالا می نویسیم.برای مثال :
 
 
 git remote add origin https://github.com/atefeh1378/ati.git
 
 
مرحله آخر آپلود کردن فایل های خود در گیت هاب هست با استفاده از دستور زیر :


git push origin master


اطلاعات کاربری خود را وارد می کنیم تمام شد. محتویات پوشه ما به گیت هاب اضافه شد .

حالت کلی دستور فوق :

cd Documents/
mkdir ati
cd ati/
git init
git add --all
git commit -m "some-message"
git remote add origin https://github.com/atefeh1378/ati.git
git push origin master



سوال ۴) دستوری بنویسید که مشخص نماید از لحظه روشن شدن سیستم و بوت شدن سیستم عامل چه مدت زمانی سپری شده است ؟

با استفاده از دستور زیر :

system-analyze


همچنین با دستور آپ تایم هم می توانیم بفهمیم چه مدت زمانی از لحظه روشن شدن سیستم می گذرد.
 
 uptime
 

