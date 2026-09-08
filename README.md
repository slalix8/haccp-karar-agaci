# 🛡️ Automated HACCP Decision Tree & Food Safety Verification Engine

Gıda güvenliği yönetim sistemlerinde (BRCGS v9, ISO 22000, Codex Alimentarius) tehlike analizi ve kritik kontrol noktası (CCP) belirleme süreçlerini otomatize eden Python tabanlı kural motoru.

Manuel Excel takiplerindeki insan hatasını sıfırlayarak; tehlike girdilerini okur, 4 adımlı Codex karar ağacı algoritmasını çalıştırır, CCP / oPRP sınıflandırmasını yapar ve denetime hazır biçimlendirilmiş bir Excel raporu üretir.

---

## 🚀 Temel Özellikler

* **Kural Tabanlı Karar Motoru:** Codex Alimentarius CCP karar ağacı mantığını (S1-S4 soruları) dinamik olarak işletir.
* **Risk Matrisi ve Sınıflandırma:** Olasılık ve şiddet parametrelerini değerlendirerek tehlikeleri ön elemeden geçirir.
* **Otomatik Operasyonel Parametre Eşleme:** Tespit edilen her CCP için kritik limitleri, izleme sıklığını, yöntemini ve düzeltici faaliyet prosedürlerini otomatik bağlar.
* **Denetim Uyumlu Raporlama (`openpyxl`):** Çıktı tablosunu BRCGS standartlarına uygun başlık renkleri, otomatik hücre genişlikleri ve karar türüne özel renk kodlarıyla (CCP: Kırmızı, oPRP: Sarı, PRP: Yeşil) formatlar.

---

## 🛠️ Kullanılan Teknolojiler

* **Dil:** Python 3.13+
* **Veri Manipülasyonu:** `pandas`
* **Rapor Biçimlendirme & Tasarım:** `openpyxl`
* **Standartlar:** Codex Alimentarius, BRCGS Food Safety Issue 9, ISO 22000:2018

---

## 📁 Proje Yapısı

```text
├── tehlike_listesi.xlsx        # Girdi: Proses adımları ve karar ağacı yanıtları
├── haccp_analiz.py             # Analiz ve stil formatlama motoru
├── haccp_plani_final.xlsx      # Çıktı: Formatlanmış BRCGS uyumlu HACCP planı
└── README.md                   # Proje dokümantasyonu