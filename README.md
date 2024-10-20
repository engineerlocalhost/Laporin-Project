# Laporin-Project

[Anggota Kelompok 3]
- RIKY FAJAR RIZKY      043263751 
- FAHRI MUHAMAD         043958719
- MUHAMMAD RISWAN       043967829
- ANJANI AYU NINGTYAS   044017788
- RAFLI RAMZI HIDAYAT   044491675
------------------------------------------------------
[Struktur LaporinApp]

/LaporinApp
│
├── /android                # Folder untuk proyek Android
│
├── /ios                    # Folder untuk proyek iOS
│
├── /src                    # Folder utama sumber kode
│   ├── /assets             # Folder untuk gambar, ikon, dan aset lainnya
│   │   ├── /images         # Folder untuk gambar
│   │   └── /icons          # Folder untuk ikon
│   │
│   ├── /components         # Folder untuk komponen Vue reusable
│   │   ├── Header.vue      # Komponen header
│   │   ├── Footer.vue      # Komponen footer
│   │   └── KeluhanCard.vue # Komponen untuk menampilkan keluhan
│   │
│   ├── /pages              # Folder untuk halaman aplikasi
│   │   ├── Home.vue        # Halaman utama untuk melaporkan keluhan
│   │   ├── StatusKeluhan.vue # Halaman untuk memantau status keluhan
│   │   └── Profile.vue     # Halaman untuk profil pengguna (jika ada)
│   │
│   ├── /router             # Folder untuk mengatur rute aplikasi
│   │   └── index.js        # File pengaturan rute aplikasi
│   │
│   ├── /store              # Folder untuk Vuex store (jika menggunakan state management)
│   │   ├── index.js        # File utama store
│   │   └── modules         # Folder untuk modul store jika dibutuhkan
│   │
│   ├── /services           # Folder untuk API dan layanan
│   │   └── api.js          # File untuk mengatur permintaan API
│   │
│   ├── /styles             # Folder untuk file CSS dan styling
│   │   └── main.css        # File CSS utama
│   │
│   ├── /utils              # Folder untuk utilitas dan fungsi bantu
│   │   └── helpers.js      # File untuk fungsi bantu
│   │
│   ├── App.vue             # File utama aplikasi Vue
│   ├── main.js             # File entry point aplikasi
│   └── index.html          # File HTML utama
│
├── /public                 # Folder untuk file statis
│   └── favicon.ico         # Ikon favicon aplikasi
│
├── .gitignore              # File untuk mengabaikan file dan folder tertentu di Git
├── capacitor.config.json    # Konfigurasi Capacitor
├── package.json            # File konfigurasi NPM dan dependensi
├── vue.config.js           # Konfigurasi Vue CLI
└── README.md               # Dokumen penjelasan proyek

# Installasi
#LINUX
Install NPM : sudo apt install npm -y  
Install VUE : sudo npm install -g @vue/cli 
Install IONIC : sudo npm install -g @ionic/cli 
Creat Project : sudo ionic start LaporinApp blank --type vue
Masuk Ke dalam folder Project
Run Project : sudo ionic serve  
------------------------------
install semver untuk menjalankan app : npm install -g @ionic/lab semver

#WINDOWS
Install NPM : pip install npm
Install NODjs : https://nodejs.org/en/download/prebuilt-installer
Cek version nodejs dan npm yang sudah terinstall : node -v atau npm -v
Install VUE : npm install -g @vue/cli 
Install IONIC : npm install -g @ionic/cli 
Creat Project : ionic start LaporinApp blank --type vue
Masuk Ke dalam folder Project
Run Project : ionic serve  
------------------------------
install semver untuk menjalankan app : npm install -g @ionic/lab semver

============================
Disable no-sanbox vscode : code --no-sandbox --disable-gpu-sandbox --user-data-dir=/root/.vscode/
