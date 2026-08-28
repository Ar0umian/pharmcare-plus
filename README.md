<div align="center">

# 💊 Pharmacare+ 
**An Intelligent System for Drug Interaction Detection and Management** *نظام ذكي متكامل لاستكشاف وإدارة التداخلات الدوائية باستخدام الذكاء الاصطناعي*

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Framework-lightgrey.svg)](https://flask.palletsprojects.com/)
[![Scikit-learn](https://img.shields.io/badge/Scikit-Learn-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

</div>

---

## 🎥 Demonstration | العرض التوضيحي

> 
<div align="center">
    
  <img src="https://github.com/Ar0umian/demo/blob/443d0ffb5594db64a8dfbf68127e4c41207ca8cf/Pharmcare%2B%20demo.gif" alt="Pharmacare+ Project Preview" />

</div>

---

## 🇸🇦 نبذة عن المشروع (Arabic Overview)
**Pharmacare+** هو نظام ذكي لمشروع تخرج يهدف إلى تعزيز سلامة المرضى والارتقاء بكفاءة الرعاية الصحية. يعتمد النظام على تقنيات متطورة في مجال تحليل البيانات والذكاء الاصطناعي (AI) لاستكشاف التداخلات الدوائية بدقة عالية.

### ⚙️ البنية التقنية وسير العمل
* **التدريب الآلي (`train_model.py`):** جلب آلاف المقالات الطبية من **PubMed**، وتطبيق تصنيف دلالي ذكي بناءً على الكلمات المفتاحية، ثم تدريب نموذج **Logistic Regression** (مع موازنة الفئات لضمان دقة عالية) باستخدام مكتبة `Scikit-learn`.
* **الخادم الخلفي (`app.py`):** واجهة برمجة تطبيقات (API) مبنية بإطار عمل **Flask**، تتلقى أسماء الأدوية، تستعلم عن المقالات الطبية ذات الصلة، وتُمررها للنموذج للتنبؤ بمستوى الخطورة.
* **الواجهة الأمامية (`index.html` & `script.js`):** تصميم تفاعلي سلس يوفر اقتراحات تلقائية لأسماء الأدوية، ويفصل تماماً بين صناديق التحذير والنتائج لتقديم تجربة مستخدم ممتازة.

---

## 🇬🇧 Project Overview (English Overview)
**Pharmacare+** is an intelligent graduation project system designed to enhance patient safety and improve healthcare efficiency. The application utilizes sophisticated techniques in data analytics and Artificial Intelligence (AI) to accurately detect and manage potential drug-drug interactions.

### ⚙️ Technical Architecture & Pipeline
* **Machine Learning Pipeline (`train_model.py`):** Fetches thousands of medical articles from **PubMed**, applies smart semantic labeling based on keywords, and trains a balanced **Logistic Regression** model using `Scikit-learn`.
* **Backend API (`app.py`):** A robust **Flask** API that processes drug inputs, fetches relevant interaction papers, and evaluates them through the trained AI model.
* **Frontend Interface (`index.html` & `script.js`):** A clean, responsive UI featuring live drug name auto-suggestions and dynamic interaction result rendering for optimal user experience.

---

## 🚀 دليل التشغيل والتثبيت (Setup Guide)

### 1. المتطلبات الأساسية (Prerequisites)
تأكد من تثبيت **Python** على جهازك، ثم قم بتثبيت المكتبات اللازمة بتنفيذ الأمر التالي في موجه الأوامر (Terminal):
```bash
pip install flask flask-cors scikit-learn pandas joblib imbalanced-learn biopython
