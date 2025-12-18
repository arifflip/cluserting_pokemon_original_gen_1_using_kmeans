# POKÉMON CLUSTERING (GEN 1)

DESKRIPSI
Proyek ini menerapkan unsupervised clustering (K-Means) pada 151 Pokémon Generasi 1 menggunakan base stats yang diambil dari PokeAPI. Tujuannya adalah menemukan cluster Pokémon berbasis statistik pokemon tersebut.

DATA
Sumber: PokeAPI
Limitation: Hanya Generasi 1 (151 Pokémon)
Fitur yang digunakan:

FEATURES
* hp
* attack
* defense
* special_attack
* special_defense
* speed

METODOLOGI
Algoritma: K-Means
Jumlah cluster: 4
Preprocessing: hanya menggunakan fitur numerik tanpa scaling, karena seluruh base stats berada pada skala yang sama
Output:

* Cluster_Label
* cluster_name

RINGKASAN CLUSTER (BERDASARKAN PERILAKU CENTROID)

The Speedsters (~29%)
Pokémon dengan speed tinggi dan offensive stats kuat. Mengandalkan keunggulan tempo dengan menyerang lebih dulu sebelum lawan bereaksi.

The Tanks & Bruisers (~20%)
Didominasi defense yang sangat tinggi dengan attack yang solid namun speed rendah. Dirancang untuk menerima serangan lalu membalas secara efektif.

The Commoners / Un-evolved (~35%)
Seluruh base stats relatif rendah dan merata. Umumnya merupakan Pokémon tahap awal atau yang belum berevolusi.

The Heavy Armor (~15%)
Memiliki hp, defense, dan special_defense yang tinggi. Fokus utama pada daya tahan, bukan kecepatan atau inisiatif.

IMPROVEMENT
1. Ada testing comparasi perforamce K-Means dengan mencoba feature scaling.
2. Menambahkan Attribut pokemon type  beserta jumlah strong dan weaknessnya terhadap tipe lain.

TECH STACK
Python
Pandas
NumPy
Scikit-learn
PokeAPI
