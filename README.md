# رائدات المستقبل — موقع تسجيل التحفيز

- `index.html` — الموقع.
- `report-template.xlsx` — قالب ملف التقارير (بدون أسماء)، يملؤه الموقع عند «تنزيل ملف التقارير».
- `api/data.js` — واجهة البيانات (تحفظ في Upstash Redis).
- قائمة الموظفات الأولية داخل `api/data.js`، تُنسخ إلى قاعدة البيانات عند أول تشغيل فقط.

## متغيرات البيئة في Vercel
- `APP_PIN` — رمز الدخول.
- `KV_REST_API_URL` و `KV_REST_API_TOKEN` (أو `UPSTASH_REDIS_REST_URL` و `UPSTASH_REDIS_REST_TOKEN`) — تُضاف تلقائيًا عند ربط قاعدة Upstash بالمشروع.

بعد تغيير أي متغير بيئة: Deployments ← آخر نشر ← Redeploy.
