# Setup dan Init
Git konigurasi, inisialisasi dan cloning Git.

| Perintah | Keterangan |
| -- | -- |
| `git config [key] [value]` | Menetapkan nilai config di repositori |
| `git config --global [key] [value]` | Menetapkan nilai konfigurasi global untuk user |
| `git init` | Menginisialisasi direktori yang ada sebagai repositori git |
| `git clone [url]` | Clone repositori git dari URL |
| `git help [command]` | mendapatkan bantuan di setiap perintah git |

# Stage dan Snapshot
Bekerja dengan snapshot dan stage area git.

| Perintah | Keterangan |
| -- | -- |
| `Git status` | menunjukkan status apa yang di stage untuk selanjutnya melakukan commit dan apa yang diubah dalam direktori kerja Anda. |
| `git add [file]` | menambahkan file seperti yang terlihat sekarang untuk berikutnya di commit (stage) |
| `Git reset [file]` | reset staging area untuk sebuah file sehingga perubahan tidak dalam commit Anda berikutnya (unstage). |
| `git diff` | diff dari apa yang berubah tapi tidak pada stage |
| `git diff --staged` | diff dari apa yang distaged tetapi belum dicommit |
| `git commit` | commit konten stage Anda sebagai commit snapshot baru. |
| `git rm [file]` | Menghapus file dari working directory anda dan unstage. |
| `git gui` | tcl / tk program GUI untuk membuat semua perintah sederhana |

# Baranch dan Merge
Bekerja dengan Git percabangan dan stash

| Perintah | Keterangan |
| -- | -- |
| `git branch` | List cabang anda, tanda * akan muncul di sebelah cabang yang aktif. |
| `git branch [nama-baranch]` | Membuat cabang baru pada saat commit. |
| `git checkout [branch]` | Beralih ke cabang lain, memeriksanya ke working direktory anda. |
| `git checkout –b [branch]` | Membuat cabang baru dan langsung beralih ke cabang tersebut |
| `git merge [branch]` | Menggabung cabaing lain menjadi satu ke cabang yang sedang aktif dan merekam merge sebagai commit. |
| `git log` | Menampilkan log commit. |
| `git stash` | Menyimpan di sisi lain modifikasi saat ini tanpa commit dalam working directory sementara. |
| `git stash apply` | Mendaftar ulang perubahan yang distash terakhir. |

# Share dan Update
Mengambil, menggabung dan bekerja dengan update ke repositori lain.

| Perintah | Keterangan |
| -- | -- |
| `git remote add [alias] [url]` | Menambahkan git URL sebagai alias |
| `git fetch` | Mengambil semua cabang dari git remote |
| `git merge [alias]/[branch]` | menggabungkan cabang pada server ke dalam cabang Anda yang sedang aktif untuk medapatkan pembaharuan |
| `git push [alias] [branch]` | push pekerjaan di cabang Anda untuk memperbarui cabang di remote git repositori. |
| `git pull` | Mengambil dari URL yang terlacak oleh cabang saat ini dengan segera mencoba untuk menggabung dari cabang yang terlacak. |

# Inspect dan compare
Meneliti log, diffs dan informasi objek.

| Perintah | Keterangan |
| -- | -- |
| `git log` | menunjukkan sejarah commit untuk cabang yang sedang aktif |
| `git log branchB..branchA` | menunjukkan commit pada branchA yang tidak pada branchB |
| `git log --follow [file]` | menunjukkan commit dari perubahan file, bahkan mengganti nama. |
| `git diff branchB...branchA` | menunjukkan diff dari apa yang ada di branchA yang tidak branchB |
| `Git show [SHA]` | menunjukkan objek dalam Git dalam format yang dapat terbaca oleh manusia. |
| `gitx ` | tcl Program / tk untuk menampilkan log commit dalam GUI. |
