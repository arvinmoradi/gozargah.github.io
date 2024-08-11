<h1>بک آپ و ریستور پنل مرزبان با ابزار WinSCP و Terminal برای دیتابیس SQLite و MySQL</h1>
<p>برای این کار به برنامه WinSCP و یک محیط ترمینال نیاز داریم که در اینجا از Termius استفاده شده است</p>
<p>وارد برنامه شده و از قسمت new site ، اطلاعات مربوط به سرور خود را وارد کنید</p>
<code>Protocol : SFTP</code> <br>
<code>Host name : آی پی سرور</code> <br>
<code>Port : پورت SSH</code> <br>
<code>Username : نام کاربری ورود به سرور</code> <br>
<code>Password : رمزعبور ورود به سرور</code> <br>
<h3>چرا WinSCP و Terminal ؟ </h3>
<p>با WinSCP فایل‌ها را زیپ ، دانلود و آپلود می‌کنیم و با محیط Terminal فایل‌های زیپ آپلود شده را استخراج می‌کنیم چون استخراج کردن فایل‌ها با WinSCP باعث به وجود آمدن ارور میشه و بازگردانی به درستی انجام نمیشه</p>
<p>در دیتابیس sqlite می‌توانیم دو فایل db.sqlite3 و xray_config.json را دانلود و هنگام بازگردانی همان فایل‌ها را جایگزین کنیم ولی در دیتابیس MySQL با این روش به ارور می‌خوریم و قابل انجام نیست.</p>
<p>البته در این آموزش برای هر دو دیتابیس از روش زیپ کردن و استخراج کردن استفاده شده تا به هیچ اروری برخورد نکنیم</p>
<br>
<br>
<p>با این دستور یک فایل با فرمت tar.gz را از حالت زیپ خارج می‌کنیم</p>
<code>tar -xzvf filename.tar.gz</code>
<p>به جای filename.tar.gz باید اسم فایل خودتان را بنویسید که انتخاب کردین برای مثال یک فایل به اسم arm.tar.gz باید با این دستور استخراج شود</p>
<code>tar -xzvf arm.tar.gz</code>
<h2>Database SQLite</h2>
<p>در محیط سرور قبل از هر کاری وارد مسیر زیر می شویم (WinSCP) چون فایل‌ها را از این مسیر دانلود و به این مسیر آپلود می‌کنیم</p>
<code>/var/lib/marzban</code> <br>
<a href="https://youtu.be/Cf4NUhWBAg0" target="_blank" style="text-decoration:none;">مشاهده آموزش در یوتیوب</a>
<h2>Database MySQL</h2>
<p>در محیط سرور قبل از هر کاری وارد مسیر زیر می شویم (WinSCP) چون فایل‌ها را از این مسیر دانلود و به این مسیر آپلود می‌کنیم</p>
<code>/var/lib/marzban</code>
<p>اگر به هر دلیلی پنل را پاک کردید و می‌خواهید فایل‌ها را بازگردانی کنید اول باید دیتابیس را به MySQL تغییر دهید و بعد کارهای لازم را برای بازگردانی انجام دهید</p>
<a href="https://youtu.be/fivM6z55VtA" target="_blank" style="text-decoration:none;">مشاهده آموزش در یوتیوب</a> <br>
