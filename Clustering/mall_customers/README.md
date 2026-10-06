# Mall Customer Segmentation — mijozlarni guruhlash

Do'kon mijozlarini yillik daromad va xarajat ko'rsatkichi asosida guruhlarga ajratish (clustering). Bu yerda `y` (javob) yo'q — model o'xshash mijozlarni o'zi topadi.

## Fayllar

- `mall_customers.ipynb` — asosiy notebook

## Dataset

Kaggle'ning "Mall Customer Segmentation Data" dataseti (`Mall_Customers.csv`, 200 mijoz). Notebook'ni ishga tushirish uchun shu faylni Kaggle'dan yuklab, Drive'ingizga joylashtiring va notebook ichidagi `path`ni moslang.

## Nima qilindi

- EDA (bu dataset toza, missing value yo'q)
- `Annual Income` va `Spending Score` orasidagi bog'liqlikni scatter plot orqali ko'rish
- Elbow Method bilan optimal klaster sonini (k=5) topish
- K-Means (k=5) bilan mijozlarni guruhlash va natijani rangli grafikda ko'rsatish

## Natija

Besh guruh chiqdi: tejamkor mijozlar, kam pul bilan ko'p xarid qiladiganlar, o'rtacha guruh, puli bor lekin kam xarid qiladiganlar, va eng qimmatli mijozlar (yuqori daromad + yuqori xarajat). Bu real hayotda har bir guruhga alohida marketing strategiyasi qurish uchun foydali bo'ladi.
