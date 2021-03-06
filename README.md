# Bahan Ajar Desktop Programming 2019
Materi pembelajaran Python untuk AMCC divisi Desktop Programming 2019

## Materi Pembahasan Pertemuan 1
1. GitHub
2. Bash/Terminal
3. SSH (Secure Shell)
4. Git
5. Kolaborasi Projek

### 1. GitHub
1. Mendaftar di github menggunakan email students amikom.
2. Verify akun github yang terkirim ke email kamu.

### 2. Bash/Terminal
Belajar perintah dasar dari bash/terminal

### 3. SSH (Secure Shell)
Untuk melakukan pembuatan `SSH Key`, ikutin langkah-langkah berikut:
1. Buka terminal (Linux) dan GitBash (Windows)
2. ketikan `ssh-keygen` maka akan muncul pertanyaan seperti dibawah ini, hal ini memastikan tempat dimana `SSH Key` disimpan, tekan <kbd>Enter</kbd> untuk menyimpan secara default.
```bash
Generating public/private rsa key pair.
Enter file in which to save the key (/home/genpati/.ssh/id_rsa):
```
3. lalu muncul pertanyaan seperti ini, artinya, pengguna diminta untuk memasukan kata kunci khusus untuk `SSH Key` yang akan di buat, tekan <kbd>Enter</kbd> untuk menyimpan secara default.
```bash
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
```
4. kamu berhasil membuat `SSH Key`
```bash
Your identification has been saved in /home/genpati/.ssh/id_rsa.
Your public key has been saved in /home/genpati/.ssh/id_rsa.pub.
The key fingerprint is:
SHA256:xxXXx/xXxXU5hHgGQEGVCI7Y2IDDjoBie8joq0XxXx genpati@genpati
The key's randomart image is:
+---[RSA 3072]----+
|#@.+.            |
|&.*.o  .         |
|**x=... .        |
|o=*..x.  .       |
|+o o.  .S.       |
|.oo     o        |
|+XX. . .         |
|+.o.. .          |
|..xX.            |
+----[SHA256]-----+

```
5. menambahkan `SSH Key` ke akun GitHub bisa ikuti caranya [disini][1]
6. copy `SSH Key` dengan cara `cat ~/.ssh/id_rsa.pub` lalu select dan copy isi yang muncul pada terminal
7. masuk ke akun github, lalu ke profile > settings > SSH & GPG > Add Key, lalu paste `SSH Key` yang sudah di copy lalu Save Key
8. Inisialisasi akun pada git
```bash
$ git config --global user.email "david.rigan@students.amikom.ac.id"
$ git config --global user.name "David Rigan"
```
### 4. Git
#### Install Git Client
1. Untuk client windows, install terlebih dahulu [Git Bash](https://git-scm.com/downloads). Tutorial lebih lanjut ada [disini](https://git-scm.com/book/id/v1/Memulai-Git-Menginstall-Git#Menginstall-pada-Sistem-Operasi-Windows)
2. Seting identitas pengguna
```bash
$ git config --global user.name "David Rigan"
$ git config --global user.email david.rigan@students.amikom.ac.id
```
3. Pastikan akun settingan sudah berhasil dengan cek dengan cara
```bash
$ git config --list
user.name=David Rigan
user.email=david.rigan@students.amikom.ac.id
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
...
```

#### 4.1 Clone Repository
1. pada halaman ini, klik clone repository > copy SSH
2. Buka Terminal (Linux) atau GitBash (Windows), lalu clone Repository dengan cara
```bash
$ git clone git@github.com:dvrg/dp-2019.git
```
3. untuk pertamkali clone, fingerprint akan didaftarkan ke komputer kamu dan konfirmasi penambahan itu dengan `yes`
```bash
Cloning into 'dp-2019'...
The authenticity of host 'github.com (13.229.188.59)' can't be established.
RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes

```
4. maka repository akan tercopy ke lokal komputer kamu.

#### 4.2 Melakukan Perubahan
1. saat ingin menambahkan file baru pada git, caranya `git add Materi-2.md` atau jika file barunya banyak, bisa diganti menjadi `git add .`
2. saat ingin menambahkan perubahan pada git, caranya `git commit -am "pesan perubahan"`


#### 5.Kontribusi Projek

catatan : daftar perintah (git)[https://github.com/joshnh/Git-Commands]
---

Sumber :
[https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
[1]:https://help.github.com/en/articles/adding-a-new-ssh-key-to-your-github-account

---
Kontributor Proyek Ini:
+ David Rigan
+ Agnes peby thalia mencoba nih belajar git hub
+ Yanuar yayan
+ Salsabila

