# Alur Kerja Dasar Git
Untuk mengawali git repositori baru, kemudian
stage semua file ke dalam direktori dan akhirnya
commit snapshot awal.

```shell
$ git init
$ git add .
$ git commit –m ‘commit awal’
```
Membuat cabang baru bernama `FeatureA`,
kemudian melakukan `checkout` untuk mengaktifkan
cabang, kemudian lakukan perubahan dan `stage`
beberapa file dan terakhir `commit` *snapshot* baru.

```shell
$ git branch featureA
$ git checkout featureA
  (edit files)
$ git add (files)
$ git commit –m ‘menambahkan feature A’
```
Beralih kembali ke `branch master`, mengembalikan
perubahan `featureA` yang baru saja dibuat,
kemudian mengedit beberapa *file* dan `commit` perubahan
baru anda secara langsung dalam kontek cabang `master`.

```shell
$ git checkout master
$ (edit files)
$ git commit –a –m ‘perubahan files’
```

Menggabungkan perubahan `featureA` kedalam kontek
cabang `master`, menggabung semua pekerjaan anda,
terakhir hapus cabang `featureA`.

```shell
$ git merge featureA
$ git branch –d featureA
```
