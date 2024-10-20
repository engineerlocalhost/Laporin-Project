<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Riwayat Pelaporan</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <ion-list>
        <ion-item v-for="(keluhan, index) in riwayatKeluhan" :key="index">
          <ion-label>
            <h2>{{ keluhan.judul }}</h2>
            <p>{{ keluhan.deskripsi }}</p>
            <p>Status: {{ keluhan.status }}</p>
          </ion-label>
        </ion-item>
      </ion-list>
    </ion-content>
  </ion-page>
</template>

<script>
export default {
  data() {
    return {
      riwayatKeluhan: [
        {
          judul: 'Jalan Rusak',
          deskripsi: 'Jalan rusak di depan kantor kecamatan.',
          status: 'Sedang Diproses',
        },
        {
          judul: 'Lampu Jalan Mati',
          deskripsi: 'Lampu jalan mati di RT 02 RW 03.',
          status: 'Ditindaklanjuti',
        },
      ],
    };
  },
};
</script>
