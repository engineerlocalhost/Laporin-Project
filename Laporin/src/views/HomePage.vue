<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Pelaporan Keluhan</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-list>
        <ion-item>
          <ion-label position="floating">Judul Keluhan</ion-label>
          <ion-input v-model="judulKeluhan"></ion-input>
        </ion-item>

        <ion-item>
          <ion-label position="floating">Deskripsi Keluhan</ion-label>
          <ion-textarea v-model="deskripsiKeluhan"></ion-textarea>
        </ion-item>

        <ion-item>
          <ion-label position="floating">Lokasi</ion-label>
          <ion-input v-model="lokasi"></ion-input>
        </ion-item>

        <ion-item>
          <ion-label>Tambahkan Foto</ion-label>
          <input type="file" @change="handleFileUpload" />
        </ion-item>

        <ion-button expand="full" @click="laporkanKeluhan">Laporkan</ion-button>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script>
export default {
  data() {
    return {
      judulKeluhan: '',
      deskripsiKeluhan: '',
      lokasi: '',
      foto: null,
    };
  },
  methods: {
    handleFileUpload(event) {
      this.foto = event.target.files[0];
    },
    laporkanKeluhan() {
      // Logic untuk mengirim data ke server atau API
      console.log({
        judul: this.judulKeluhan,
        deskripsi: this.deskripsiKeluhan,
        lokasi: this.lokasi,
        foto: this.foto,
      });
    },
  },
};
</script>
