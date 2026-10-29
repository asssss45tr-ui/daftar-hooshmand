# دفتر حساب هوشمند مغازه

برنامه‌ی مدیریت بدهی مشتریان؛ تک‌فایل و آفلاین.

- `web/daftar-hooshmand.html` — نسخه‌ی مرورگر (با `python -m http.server`)
- `app/` — پوسته‌ی اندروید (WebView) که همان فایل را داخل `app/src/main/assets/index.html` دارد
- با هر `git push` روی شاخه‌ی main، GitHub Actions فایل نصبی را می‌سازد:
  `https://github.com/<حساب>/<مخزن>/releases/download/latest/daftar-hooshmand.apk`

## تغییر برنامه
فایل HTML را ویرایش کن و **هر دو نسخه** را هم‌سان نگه دار:
`cp web/daftar-hooshmand.html app/src/main/assets/index.html`

## نکته‌ها
- کلید امضا (`app/stable.jks`) ثابت است تا هر نسخه روی قبلی نصب شود و اطلاعات نماند. آن را حذف نکن.
- اطلاعات داخل خود اپ ذخیره می‌شود؛ قبل از حذف اپ حتماً از منوی «پشتیبان‌گیری» فایل پشتیبان بگیر.
