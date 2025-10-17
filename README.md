# Data GeoJSON Jalan Kelurahan Cipageran 🗺️

File **`cipageran.geojson`** berisi representasi digital jaringan jalan di wilayah **Kelurahan Cipageran, Kota Cimahi, Jawa Barat**, dalam format **GeoJSON (RFC 7946)**.  
Data ini menggambarkan ruas-ruas jalan utama dan gang di area sekitar koordinat pusat **6.8510° LS, 107.5416° BT**.  
Setiap ruas jalan direpresentasikan sebagai **LineString**, yaitu garis yang terbentuk dari kumpulan titik koordinat (longitude dan latitude) yang mengikuti bentuk jalan di lapangan.

---

## 🗺️ Deskripsi Isi File

File ini memiliki struktur utama berupa **FeatureCollection**, yang berisi kumpulan fitur (feature) dengan tipe geometri **LineString**.  
Setiap fitur merepresentasikan satu ruas jalan atau gang yang terdapat di wilayah Cipageran.

Komponen utama dalam file ini meliputi:

### 1. `type`
Menunjukkan tipe utama dari dokumen GeoJSON.  
Nilainya adalah `"FeatureCollection"`, yang berarti file ini berisi sekumpulan fitur geospasial.

### 2. `features`
Merupakan array yang menampung setiap ruas jalan (fitur individu).  
Setiap elemen di dalamnya memiliki dua bagian penting: **`properties`** dan **`geometry`**.

---

## 🧾 Penjelasan Atribut Fitur

### 🔸 `type`
Nilainya `"Feature"`, menandakan bahwa elemen tersebut merupakan satu objek spasial yang berdiri sendiri.

## 🌍 Atribut Geometri (`geometry`)

Bagian ini mendeskripsikan bentuk dan posisi geografis setiap ruas jalan.

| Elemen | Deskripsi |
|--------|------------|
| **`type`** | Nilainya `"LineString"`, menunjukkan bahwa fitur ini berupa garis yang terbentuk dari serangkaian titik. |
| **`coordinates`** | Daftar pasangan nilai `[longitude, latitude]` yang merepresentasikan posisi setiap titik di sepanjang jalan. Koordinat disusun berurutan sesuai arah jalan di peta. |

Contoh struktur geometri:
```json
"geometry": {
  "type": "LineString",
  "coordinates": [
    [107.5412, -6.8515],
    [107.5418, -6.8511],
    [107.5423, -6.8506]
  ]
}
