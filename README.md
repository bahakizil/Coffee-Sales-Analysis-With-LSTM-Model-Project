# Kahve Satış Tahmininde Derin Öğrenme: Günlük Satışların Analizi ve Geleceğin Öngörülmesi

## İçindekiler
- [Proje Hakkında](#proje-hakkında)
- [Veri Seti](#veri-seti)
- [Kullanılan Yöntemler](#kullanılan-yöntemler)
- [Görselleştirmeler ve Analizler](#görselleştirmeler-ve-analizler)
- [Sonuçlar ve Uygulama Alanları](#sonuçlar-ve-uygulama-alanları)
- [Gelecek Çalışmalar](#gelecek-çalışmalar)
- [Requirements](#requirements)
- [Installation](#installation)

## Proje Hakkında
Bu projede, bir kahve dükkanının günlük satış verileri kullanılarak satış trendlerini analiz etmek ve gelecekteki karları tahmin etmek amaçlanmıştır. Proje kapsamında, zaman serisi analizi ve derin öğrenme modelleri kullanılmıştır.

## Veri Seti
Veri seti, kahve dükkanındaki satış verilerini içermektedir. Aşağıdaki sütunlar yer almaktadır:
- datetime: Satışın gerçekleştiği tam tarih ve saat
- coffee_name: Satılan kahve türü

Ek olarak, İstanbul'un hava durumu verileri de kullanılmıştır. Hava durumu verileri şu bilgileri içermektedir:
- DateTime: Hava durumu verisinin tarihi ve saati
- MaxTemp: Günün maksimum sıcaklığı
- MinTemp: Günün minimum sıcaklığı
- Condition: Hava durumu koşulu

Veri seti: [Kaggle - Coffee Sales](https://www.kaggle.com/datasets/ihelon/coffee-sales)

## Kullanılan Yöntemler
Proje kapsamında aşağıdaki adımlar izlenmiştir:
1. **Veri Hazırlama:** Veriler, uygun formatta yüklenmiş ve gerekli ön işlemler yapılmıştır.
2. **Zaman Serisi Analizi:** Günlük toplam satış miktarları ve kahve türleri analiz edilmiştir.
3. **Derin Öğrenme Modeli:** Gelecekteki karları tahmin etmek için PyTorch ile bir LSTM (Long Short-Term Memory) modeli kullanılmıştır.
4. **Görselleştirme:** Satış verileri çeşitli grafiklerle görselleştirilmiştir.

## Görselleştirmeler ve Analizler
Projede kullanılan ve oluşturulan görselleştirmeler şunlardır:
- **Günlük Toplam Satış Bar Grafiği:** Günlük toplam satış miktarları bar grafiği ile görselleştirilmiştir.
- **Kahve Türlerinin Günlük Dağılımı Pasta Grafiği:** Kahve türlerinin günlük satış dağılımı pasta grafiği ile gösterilmiştir.
- **Kahve Türlerinin Günlük Satış Trendi Çizgi Grafiği:** Kahve türlerinin günlük satış trendleri çizgi grafiği ile görselleştirilmiştir.
- **Günlük Toplam Satış Kutu Grafiği:** Günlük toplam satış miktarlarının aylık dağılımı kutu grafiği ile gösterilmiştir.
- **Hava Durumuna Göre Satış Analizi:** Hava koşullarının kahve satışları üzerindeki etkisi analiz edilmiştir.
- **Sıcaklık Aralıklarına Göre Satış Violin Grafiği:** Farklı sıcaklık aralıklarının kahve satışları üzerindeki etkisi incelenmiştir.

## Sonuçlar ve Uygulama Alanları
Bu proje, kahve dükkanları için çeşitli faydalar sağlamaktadır:
- **Pazarlama ve Satış Stratejileri:** Belirli zaman dilimlerinde özel kampanyalar düzenlenebilir ve müşteri davranışları analiz edilerek yeni ürünler tanıtılabilir.
- **Stok Yönetimi:** Talep tahmini yapılabilir ve atık miktarı azaltılabilir.
- **Operasyonel Verimlilik:** Yoğun satış dönemleri belirlenerek, çalışan vardiya planlamaları daha verimli hale getirilebilir ve operasyonel maliyetler düşürülebilir.
- **Müşteri Memnuniyeti:** Müşterilere kişiselleştirilmiş hizmet sunulabilir ve sadakat programları geliştirilebilir.

## Gelecek Çalışmalar
Gelecekte, bu proje üzerinde yapılabilecek iyileştirmeler şunları içermektedir:
- **Kullanıcı Dostu Arayüz:** Projeyi, kullanıcıların verileri kolayca yükleyip analiz sonuçlarını görselleştirebileceği bir arayüz ile donatmak.
- **Dinamik Hava Durumu Verileri:** Hava durumu verilerini belirli bir CSV dosyası yerine, her konuma özel ve daha çeşitli parametreleri içerecek bir hava durumu API'si ile sağlamak.
- **Gelişmiş Veri Analizleri:** Satışı etkileyebilecek farklı parametreler ve unsurları projeye entegre ederek, daha derin analizler ve çeşitli çıkarımlar elde etmek.

## Requirements

- pandas==2.0.3
- numpy==1.24.3
- matplotlib==3.7.1
- scikit-learn==1.2.2
- torch==2.0.1
- requests==2.31.0
- seaborn==0.12.2

## Installation

To install the required packages, run:

```bash
pip install -r requirements.txt
