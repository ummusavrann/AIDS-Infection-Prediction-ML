# 🩺 AIDS Virüsü Enfeksiyon Tahmini ve Model Optimizasyonu

Bu proje, makine öğrenmesi yöntemleri kullanarak HIV/AIDS enfeksiyon durumunu tahmin etmek amacıyla geliştirilmiştir. Çalışma; veri görselleştirmeden (EDA) başlayıp, dengesiz veri sorununun çözümüne ve modelin açıklanabilirliğine kadar uçtan uca bir süreci kapsamaktadır.

---

## 📂 Proje İçeriği
* **`ML_Proje.Rmd`**: R ve Quarto kullanılarak hazırlanan analiz kodları.
* **`ML_Proje.pdf`**: İstatistiksel tabloları ve grafik yorumlarını içeren kapsamlı teknik rapor.
* **`Presentation.pdf`**: Proje sonuçlarının ve stratejik bulguların özetlendiği sunum dosyası.

---

## 📊 Öne Çıkan Teknik Detaylar

### 1. Veri Ön İşleme ve İstatistiksel Analiz (EDA)
* 2139 gözlem üzerinden yapılan analizlerde, CD4/CD8 marker seviyelerinin enfeksiyon üzerindeki etkileri incelenmiştir.
* Hedef değişkendeki (%76 negatif - %24 pozitif) dengesizlik sorunu tespit edilmiştir.

### 2. Dengesiz Veri Çözümü: SMOTE
* Modelin yanlılığını önlemek amacıyla **SMOTE** yöntemi kullanılarak veri seti dengelenmiştir.


### 3. Model Eğitimi ve Optimizasyon
* Random Forest modelinde görülen **aşırı öğrenme (overfitting)** sorunu, **10-katlı çapraz doğrulama (10-fold Cross-Validation)** ve hiperparametre ayarları ile optimize edilmiştir.


---

## 🏆 Sonuç ve Performans Metrikleri

| Metrik | Değer |
| :--- | :--- |
| **Doğruluk (Accuracy)** | %89.2 |
| **Duyarlılık (Sensitivity)** | %88.3 |
| **Özgünlük (Specificity)** | %89.5 |
| **Hassasiyet (Precision)** | %72.8 |

## 🧠 Önemli Değişkenler (Variable Importance)
Modelin tahmin gücünü en çok etkileyen faktörler: **Tanıya kadar geçen süre (Time)**, **CD420 seviyesi**, **Tedavi durumu** ve **Semptomlar** olarak belirlenmiştir.
