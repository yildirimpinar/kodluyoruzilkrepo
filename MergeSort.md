# 🧩 Merge Sort (Birleştirmeli Sıralama)

## 🔢 Başlangıç Dizisi
[16, 21, 11, 8, 12, 22]

## 🔹 1. Adım: Diziyi ikiye böl
[16, 21, 11]   |   [8, 12, 22]

## 🔹 2. Adım: Sol ve sağ dizileri kendi içinde böl
Sol taraf: [16, 21, 11] → [16] [21, 11]
Sağ taraf: [8, 12, 22] → [8] [12, 22]

## 🔹 3. Adım: Tek eleman kalana kadar böl
Sol taraf: [21, 11] → [21] [11]
Sağ taraf: [12, 22] → [12] [22]

## 🔹 4. Adım: Birleştirme işlemleri
Sol dizi: [21] + [11] → [11, 21]
          [16] + [11, 21] → [11, 16, 21]
Sağ dizi: [12] + [22] → [12, 22]
          [8] + [12, 22] → [8, 12, 22]

## 🔹 5. Adım: Son iki alt diziyi birleştir
[11, 16, 21] + [8, 12, 22] → [8, 11, 12, 16, 21, 22]

## ✅ Sonuç
[8, 11, 12, 16, 21, 22]

## 🧮 Zaman Karmaşıklığı (Big-O)
| Durum     | Karmaşıklık |
|------------|--------------|
| En iyi     | O(n log n)  |
| Ortalama   | O(n log n)  |
| En kötü    | O(n log n)  |

Merge Sort her adımda diziyi ikiye böler (log n katman)  
ve her katmanda tüm elemanları birleştirir (n işlem).

## 💡 Ek Bilgi
- Kararlı bir sıralama algoritmasıdır.  
- “Böl ve fethet” (Divide and Conquer) stratejisiyle çalışır.  
- Avantajı: Büyük veri kümelerinde verimlidir.  
- Dezavantajı: Ek bellek kullanımı gerektirir.

👩‍💻 Hazırlayan: **Pınar**  
📚 Konu: Merge Sort - Algoritma Analizi
