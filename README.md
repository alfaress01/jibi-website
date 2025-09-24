# دليل نشر موقع app-ads.txt

## نظرة عامة

هذا الموقع يحتوي على ملف `app-ads.txt` المطلوب لتطبيق Jibi Expense Tracker. يجب رفع هذا الموقع على خدمة استضافة مجانية ليكون متاحاً على الإنترنت.

## محتويات الموقع

- `index.html` - الصفحة الرئيسية للتطبيق
- `privacy.html` - صفحة سياسة الخصوصية
- `app-ads.txt` - ملف التحقق من الإعلانات (الأهم!)

## خدمات الاستضافة المجانية الموصى بها

### 1. GitHub Pages (الأسهل والأفضل)

#### الخطوات:
1. أنشئ حساب على [GitHub.com](https://github.com)
2. أنشئ مستودع جديد باسم `jibi-website`
3. ارفع جميع ملفات مجلد `website` إلى المستودع
4. اذهب إلى Settings > Pages
5. اختر Source: Deploy from a branch
6. اختر Branch: main
7. احفظ الإعدادات

**الرابط النهائي سيكون:** `https://yourusername.github.io/jibi-website/app-ads.txt`

### 2. Netlify

#### الخطوات:
1. اذهب إلى [netlify.com](https://netlify.com)
2. أنشئ حساب مجاني
3. اسحب مجلد `website` إلى منطقة الرفع
4. سيتم نشر الموقع تلقائياً

**الرابط النهائي سيكون:** `https://random-name.netlify.app/app-ads.txt`

### 3. Vercel

#### الخطوات:
1. اذهب إلى [vercel.com](https://vercel.com)
2. أنشئ حساب مجاني
3. اربط حسابك بـ GitHub
4. ارفع المشروع من GitHub
5. سيتم النشر تلقائياً

### 4. Firebase Hosting

#### الخطوات:
1. اذهب إلى [Firebase Console](https://console.firebase.google.com)
2. أنشئ مشروع جديد
3. فعل Firebase Hosting
4. ثبت Firebase CLI: `npm install -g firebase-tools`
5. سجل دخول: `firebase login`
6. في مجلد website: `firebase init hosting`
7. انشر: `firebase deploy`

## إعداد النطاق المخصص (اختياري)

إذا كان لديك نطاق مخصص:

1. اشتر نطاق من أي مزود (مثل Namecheap, GoDaddy)
2. في إعدادات DNS، أضف CNAME record:
   - Name: www
   - Value: yourusername.github.io (أو رابط الاستضافة)
3. في GitHub Pages، أضف النطاق المخصص

## التحقق من عمل app-ads.txt

بعد النشر، تأكد من:

1. زيارة `https://yourwebsite.com/app-ads.txt`
2. التأكد من ظهور المحتوى:
   ```
   google.com, pub-1610497153546455, DIRECT, f08c47fec0942fa0
   ```
3. استخدام [أداة التحقق من Google](https://adstxt.guru/) للتأكد من صحة الملف

## إضافة الرابط في Google Play Console

1. اذهب إلى Google Play Console
2. اختر تطبيقك
3. اذهب إلى Policy > App content
4. في قسم Ads، أضف رابط app-ads.txt:
   `https://yourwebsite.com/app-ads.txt`

## إضافة الرابط في AdMob

1. اذهب إلى AdMob Console
2. اختر تطبيقك
3. اذهب إلى Settings > App settings
4. أضف Website URL: `https://yourwebsite.com`

## نصائح مهمة

- ✅ تأكد من أن ملف app-ads.txt يمكن الوصول إليه مباشرة
- ✅ لا تضع الملف في مجلد فرعي
- ✅ تأكد من أن المحتوى صحيح تماماً
- ✅ استخدم HTTPS وليس HTTP
- ✅ تأكد من عدم وجود أخطاء في الملف

## استكشاف الأخطاء

### إذا لم يعمل الملف:
1. تحقق من الرابط في المتصفح
2. تأكد من عدم وجود مسافات إضافية
3. تأكد من أن الملف نص خالص (plain text)
4. تحقق من إعدادات DNS إذا كنت تستخدم نطاق مخصص

### إذا ظهرت أخطاء في AdMob:
1. انتظر 24-48 ساعة للتحديث
2. تأكد من صحة معرف الناشر
3. تحقق من أن الملف متاح عبر HTTPS

## الدعم

إذا واجهت أي مشاكل، يمكنك:
- مراجعة [وثائق Google AdMob](https://support.google.com/admob/answer/9787919)
- استخدام [أداة التحقق](https://adstxt.guru/)
- التواصل مع دعم AdMob