# نموذج بيانات المبيعات

## الجداول
- `dim_date` بعد التاريخ
- `dim_product` بعد المنتج
- `fact_sales` حقيقة المبيعات

## العلاقات
- fact_sales[date_key] → dim_date[date_key]
- fact_sales[product_id] → dim_product[product_id]

## خطوات Power BI
1. استورد ملفات CSV من مجلد data.
2. أنشئ العلاقات أعلاه.
3. الصق المقاييس من `dax/measures.dax`.
4. ابنِ صفحة: بطاقات KPI + أعمدة حسب المنطقة + خط شهري.
