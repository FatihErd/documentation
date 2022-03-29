---
id: vi
sidebar_label: VI EDITOR
title: VI Editör
---

# Vi Editörü Kullanımı

Linux işletim sisteminde metin dosyalarını düzenlemek için kullanılır. Yazı düzenlemenin yanında komut ile işlemlerin yapılabilmesini sağlayan gelişmiş bir programdır.

## Temel VI Komutları

|              | Taşıma                                            |
| :----------: | ------------------------------------------------- |
|    **h**     | İmleci sola hareket ettirir.                      |
|    **l**     | İmleci sola hareket ettirir.                      |
|    **j**     | İmleci aşağı hareket ettirir.                     |
|    **k**     | İmleci yukarı hareket ettirir.                    |
| **[Ctrl] f** | İmleci bir sayfa ileri atar.                      |
| **[Ctrl] b** | İmleci bir sayfa geri atar.                       |
|    **^**     | İmleci bulunduğu satırdaki ilk karaktere götürür. |
|    **$**     | İmleci bulunduğu satırdaki son karaktere götürür. |
|    **G**     | İmleci dosyadaki son satıra götürür.              |
|    **nG**    | İmleci n. satıra götürür.                         |
| **[Ctrl] G** | Dosya ismini ve imlecin nerede olduğunu gösterir. |

|       | Yazı Moduna Geçme                                                                    |
| :---: | ------------------------------------------------------------------------------------ |
| **i** | İmlecin o an bulunduğu yerden itibaren yazmaya başlar.                               |
| **a** | İmlecin o an bulunduğu yerden sonraya yazmaya başlar.                                |
| **o** | İmlecin bulunduğu satırdan sonrasına yeni bir satır açılır ve yazma moduna geçer.    |
| **O** | İmlecin bulunduğu satırdan önceki satıra yeni bir satır açılır ve yazma moduna geçer |

|                           | Değiştir                                             |
| ------------------------- | ---------------------------------------------------- |
| **:%s/Ara/Degistir/flag** | Ara ve değiştir. (Flag bilgileri aşağıdaki gibidir.) |
| **g**                     | Flag Bulunan herşeyi değiştir.                       |
| **c**                     | Flag Degistirmeden önce onay ister                   |

|             | Arama                                             |
| :---------: | ------------------------------------------------- |
| **/kelime** | İmleçten sonraki yazılarda ilgili kelimeyi bulur. |
| **?kelime** | İmleçten önceki yazılarda ilgili kelimeyi bulur.  |
|    **n**    | Son yapılan aramayı devam ettir.                  |

|        | Kopyala ve Yapıştır                                            |
| :----: | -------------------------------------------------------------- |
| **yy** | İmlecin bulunduğu satırı kopyalar.                             |
| **p**  | Hafızadaki veriyi imlecin bulunduğu satırın altına yapıştırır. |

|        | Silme                                                   |
| :----: | ------------------------------------------------------- |
| **x**  | imlecin bulunduğu yerdeki karakteri siler.              |
| **dw** | İmlecin bulunduğu yerdeki kelimeyi siler. (delete word) |
| **D**  | İmlecin bulunduğu yerden satır sonuna kadar siler.      |
| **dd** | İmlecin bulunduğu satırı siler.                         |

|       | Tekrarla                                                         |
| :---: | ---------------------------------------------------------------- |
| **.** | En son yapılan ekleme, değiştirme veya silme işlemini tekrarlar. |

|          | Bir komutu Tekrarlama                 |
| :------: | ------------------------------------- |
|  **5j**  | imleci 5 satır aşağı hareket ettirir. |
| **30dd** | 30 satırı siler.                      |
| **4cw**  | imleçten itibaren 4 kelimeyi siler.   |
|  **1G**  | Dosya içindeki 1. Satıra gider.       |

|                 | Kaydetme ve Çıkma                                                       |
| :-------------: | ----------------------------------------------------------------------- |
| **:x [ENTER]**  | Değişiklikleri kaydeder ve dosyadan çıkar.                              |
| **:q [ENTER]**  | Değişiklikleri kaydetmeden dosyadan çıkar.(kaydetmek için uyarı verir)  |
| **:wq [ENTER]** | Değişiklikleri kaydeder ve dosyadan çıkar.                              |
|     **:q!**     | Değişiklikleri kaydetmeden dosyadan çıkar.(kaydetmek için uyarı vermez) |
