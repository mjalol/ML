# 🚢 Titanic: Omon Qolishni Bashorat Qilish

Birinchi shaxsiy Machine Learning loyiham — Kaggle'ning ["Titanic - Machine Learning from Disaster"](https://www.kaggle.com/competitions/titanic) dataset'i asosida classification (tasniflash) muammosi.

## Loyiha haqida

Bu loyihada yo'lovchining Titanic falokatida omon qolgan yoki qolmaganini uning demografik va bilet ma'lumotlari (jinsi, yoshi, bilet klassi, narxi va h.k.) asosida bashorat qiluvchi model qurdim. Shu bilan birga, "Women and children first" degan tarixiy qoidani real statistika bilan tekshirdim.

## Fayllar

| Fayl | Tavsif |
|---|---|
| `titanic_classification.ipynb` | Asosiy notebook — to'liq EDA, tozalash, tahlil va modellash jarayoni |
| `train.csv` / `test.csv` / `gender_submission.csv` | Kaggle'dan olingan asl datalar |

## Ishlatilgan usullar

- **EDA:** missing values tahlili, statistik ko'rsatkichlar, "Women and children first" qoidasini vizualizatsiya orqali tekshirish
- **Preprocessing:** missing value'larni to'ldirish (median/mode), Label Encoding, One-Hot Encoding, keraksiz ustunlarni olib tashlash
- **Modellar:** Logistic Regression, Random Forest
- **Feature Engineering:** `Has_Cabin`, `FamilySize`, `IsAlone`
- **Baholash:** accuracy, precision, recall, f1-score, feature importance
- **Hyperparameter tuning:** GridSearchCV (5-fold cross-validation)

## Natijalar

| Model | Accuracy |
|---|---|
| **Logistic Regression (baseline)** | **82.1%** ✅ eng yaxshi natija |
| Random Forest (baseline) | 79.9% |
| Logistic Regression + feature engineering | 81.0% |
| Random Forest (tuned) | 80.4% |

## Asosiy xulosalar

1. "Women and children first" qoidasi data orqali tasdiqlandi — ayollar va bolalarning omon qolish foizi sezilarli yuqori chiqdi, va bu `Sex`ning eng muhim feature bo'lishida ham aks etdi.
2. Kichik va oddiy datasetlarda murakkab model (Random Forest) har doim ham oddiy modeldan (Logistic Regression) yaxshiroq bo'lavermaydi.
3. Qo'shimcha feature qo'shish har doim natijani yaxshilamaydi — ba'zan multicollinearity orqali zarar ham keltirishi mumkin.

## Ishga tushirish

Notebook Google Colab uchun tayyorlangan. Ishga tushirish uchun:
1. `train.csv`, `test.csv`, `gender_submission.csv` fayllarini Google Drive'ingizga yuklang
2. Notebook'dagi `path` o'zgaruvchisini o'z papka manzilingizga moslang
3. Barcha cell'larni tartib bilan ishga tushiring

## Muallif

Mirjalol — O'zMU talabasi, ML yo'nalishida o'z-o'zini o'rgatuvchi
