# 🌳 Binary Search Tree (İkili Arama Ağacı)

## 🔢 Başlangıç Dizisi
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

---

## 🌿 Ağaç Oluşturma Aşamaları

1️⃣ **İlk eleman root olur:**
Root = 7

---

2️⃣ **5 eklenir:** 5 < 7 → sola gider.  
Yapı:
```
    7
   /
  5
```

---

3️⃣ **1 eklenir:** 1 < 7 → sola, 1 < 5 → sola.  
```
    7
   /
  5
 /
1
```

---

4️⃣ **8 eklenir:** 8 > 7 → sağa gider.  
```
    7
   / \
  5   8
 /
1
```

---

5️⃣ **3 eklenir:** 3 < 7 → sola, 3 < 5 → sola, 3 > 1 → sağa gider.  
```
      7
     / \
    5   8
   /
  1
   \
    3
```

---

6️⃣ **6 eklenir:** 6 < 7 → sola, 6 > 5 → sağa gider.  
```
      7
     / \
    5   8
   / \
  1   6
   \
    3
```

---

7️⃣ **0 eklenir:** 0 < 7 → sola, 0 < 5 → sola, 0 < 1 → sola gider.  
```
      7
     / \
    5   8
   / \
  1   6
 / \
0   3
```

---

8️⃣ **9 eklenir:** 9 > 7 → sağa, 9 > 8 → sağa gider.  
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
```

---

9️⃣ **4 eklenir:** 4 < 7 → sola, 4 < 5 → sola, 4 > 1 → sağa, 4 > 3 → sağa gider.  
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
     \
      4
```

---

🔟 **2 eklenir:** 2 < 7 → sola, 2 < 5 → sola, 2 > 1 → sağa, 2 < 3 → sola gider.  
```
      7
     / \
    5   8
   / \   \
  1   6   9
 / \
0   3
   / \
  2   4
```

---

## 🌳 Nihai Ağaç Yapısı

- **Root:** 7  
- Root’un **solunda:** 5  
- Root’un **sağında:** 8  
- 5’in **solunda:** 1  
- 5’in **sağında:** 6  
- 1’in **solunda:** 0  
- 1’in **sağında:** 3  
- 3’ün **solunda:** 2  
- 3’ün **sağında:** 4  
- 8’in **sağında:** 9  

---

## 🧠 Özet
Binary Search Tree, her yeni elemanı eklerken aşağıdaki kurala göre konumlandırır:
- **Küçük elemanlar** sol dala,  
- **Büyük elemanlar** sağ dala eklenir.  

Bu sayede arama işlemleri **O(log n)** ortalama karmaşıklıkla yapılabilir.

---

👩‍💻 Hazırlayan: **Pınar**  
📚 Konu: Binary Search Tree - Veri Yapıları  
