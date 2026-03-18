# 🏋️ Exercises Dataset

Bu repo, 433 farklı fitness egzersizine ait veri setini içermektedir. Her egzersiz için egzersiz adı, kategori, hedef kas grubu, ekipman bilgisi, açıklama, görsel ve video URL'leri bulunmaktadır.

## ⚠️ Yasal Uyarı / Disclaimer

> **Bu repo yalnızca eğitim ve araştırma amaçlıdır. Ticari kullanım kesinlikle yasaktır.**
>
> The content in this repository is provided **for educational and non-commercial purposes only**. All exercise media (images, videos) belong to their respective copyright holders. This dataset is not intended for commercial use. If you are the copyright owner and wish to have your content removed, please open an issue or contact the repository owner.
>
> Bu repodaki içerikler (görseller, videolar) ilgili telif hakkı sahiplerine aittir. İçeriklerinizin kaldırılmasını istiyorsanız lütfen bir issue açın.

---

## 📂 Klasör Yapısı

```
exercises-dataset/
├── data/
│   └── exercises.json       # 433 egzersizin tam veri seti (JSON)
├── images/                  # Egzersiz küçük resimleri (.jpg / .png)
├── videos/                  # Egzersiz animasyon videoları (.mp4)
├── download_media.py        # Medya dosyalarını indirme scripti
└── README.md
```

---

## 📊 Veri Seti İçeriği

`data/exercises.json` dosyası aşağıdaki alanları içermektedir:

| Alan | Açıklama |
|------|----------|
| `id` | Egzersizin benzersiz UUID'si |
| `name` | Egzersiz adı |
| `category` | Kas grubu kategorisi (chest, back, legs, vb.) |
| `equipment` | Kullanılan ekipman (Barbell, Dumbbell, Machine, vb.) |
| `instructions` | Egzersiz açıklaması (Türkçe) |
| `muscle_group` | İkincil kas grubu |
| `target` | Hedef kas |
| `image` | Küçük resim URL'si |
| `gif_url` | Video/animasyon URL'si |

**Toplam egzersiz sayısı:** 433

---

## 🚀 Medya Dosyalarını İndirme

Görsel ve videoları yerel olarak indirmek için `download_media.py` scriptini çalıştırın:

```bash
python3 download_media.py
```

> **Not:** Medya URL'leri imzalı Supabase URL'leridir ve süreleri dolmuş olabilir. Eğer indirme başarısız olursa URL'lerin süresi dolmuş demektir.

---

## 📋 Örnek Veri

```json
{
  "id": "c04798ba-98b3-4210-9319-0e12d10cff23",
  "name": "Bench Press (Barbell)",
  "category": "chest",
  "equipment": "Barbell",
  "instructions": "Barbell Bench Press, göğüs, omuz ve triceps kaslarını çalıştıran temel bir egzersizdir.",
  "muscle_group": "shoulders",
  "target": "Chest",
  "image": "https://...",
  "gif_url": "https://..."
}
```

---

## 🏷️ Kategoriler

Veri setinde bulunan başlıca kategoriler:

`chest` · `back` · `shoulders` · `biceps` · `triceps` · `quadriceps` · `hamstrings` · `glutes` · `calves` · `abs` · `cardio` · `forearms`

---

## 📄 Lisans

Bu proje **eğitim amaçlıdır**. Ticari kullanım için lütfen orijinal içerik sahipleriyle iletişime geçin.
