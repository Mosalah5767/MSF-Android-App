المرحلة التالية لربط Mo.F مع Google Firebase

تم وضع ملف google-services.json في المسار الصحيح app/google-services.json.
أضفنا خطوة مؤقتة في GitHub Actions لعرض SHA-1 الخاص بتوقيع نسخة debug.

ما عليك فعله:
1) ارفع محتويات المشروع إلى مستودع MSF-Android-App مع الحفاظ على المجلدات.
2) افتح GitHub > Actions وشغّل Build Android APK (أو انتظر اكتماله).
3) افتح سجل خطوة Print Android debug SHA-1 for Firebase.
4) انسخ قيمة SHA1 فقط وأرسلها هنا.

بعدها نضيف SHA-1 إلى إعدادات تطبيق Android في Firebase، ثم ننزّل google-services.json المحدّث ونكمل إضافة تسجيل الدخول والمزامنة.

مهم: حتى الآن لم نفعّل المزامنة داخل التطبيق؛ هذه المرحلة تجهّز بصمة Android المطلوبة لتسجيل الدخول الآمن عبر Google. لا تحذف التطبيق المثبت ولا تمسح بياناته.
