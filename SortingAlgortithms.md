# 🔢 Sorting Algorithms Example

Bu dosyada **Insertion Sort** ve **Selection Sort** algoritmalarının adım adım uygulanışı, zaman karmaşıklığı ve analizleri bulunmaktadır.

---

## 🧩 1️⃣ Insertion Sort

**Verilen dizi:**  
`[22, 27, 16, 2, 18, 6]`

### 🔹 Adımlar

1. `[22] | [27, 16, 2, 18, 6]`  
   → İlk eleman tek başına sıralı kabul edilir.

2. `[22, 27] | [16, 2, 18, 6]`  
   → 27, 22’den büyük, yerinde kalır.

3. `[16, 22, 27] | [2, 18, 6]`  
   → 16, 27 ve 22’nin önüne geçer.

4. `[2, 16, 22, 27] | [18, 6]`  
   → 2, tüm elemanların önüne geçer.

5. `[2, 16, 18, 22, 27] | [6]`  
   → 18, 16’dan büyük, 22’den küçük → araya yerleşir.

6. `[2, 6, 16, 18, 22, 27]`  
   → 6, 2’den sonra yerleşir.

✅ **Sonuç:**  
`[2, 6, 16, 18, 22, 27]`

---

### 🔹 Big-O Gösterimi

| Durum | Karmaşıklık |
|--------|--------------|
| Best Case | O(n) |
| Average Case | O(n²) |
| Worst Case | O(n²) |

👉 **Genel Big-O:** `O(n²)`

---

### 🔹 Time Complexity - 18 Sayısı

Sıralı dizide: `[2, 6, 16, 18, 22, 27]`  
18 dizinin **ortasında** yer alır.  

**Sonuç:**  
✅ **18 → Average Case**

---

## 🧩 2️⃣ Selection Sort

**Verilen dizi:**  
`[7, 3, 5, 8, 2, 9, 4, 15, 6]`

### 🔹 İlk 4 Adım

1. En küçük eleman **2**, 7 ile yer değiştirir.  
   → `[2, 3, 5, 8, 7, 9, 4, 15, 6]`

2. En küçük eleman **3**, zaten doğru yerde.  
   → `[2, 3, 5, 8, 7, 9, 4, 15, 6]`

3. En küçük eleman **4**, 5 ile yer değiştirir.  
   → `[2, 3, 4, 8, 7, 9, 5, 15, 6]`

4. En küçük eleman **5**, 8 ile yer değiştirir.  
   → `[2, 3, 4, 5, 7, 9, 8, 15, 6]`

✅ **İlk 4 adım sonrası dizi:**  
`[2, 3, 4, 5, 7, 9, 8, 15, 6]`

---

### ✨ Özet
- **Insertion Sort:** Elemanları tek tek alıp uygun yere yerleştirir.  
- **Selection Sort:** En küçük elemanı bulup başa alır.  
- **Big-O:** Her iki algoritma için de genelde `O(n²)`.

---

🧠 *Hazırlayan:* Pınar  
📚 *Konu:* Sorting Algorithms - Insertion & Selection Sort  
