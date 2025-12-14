Tutor By: Programmer Zaman Now

# Membuat Module
- Buat repository baru di github
- Buat modules di local:
  - Bikin folder baru
  - `go mod init github.com/FathanJundiR/go-hello-modules`
  - `git init`
  - `git branch -M main`
  - `git remote add origin link_ssh`
  - Buat file codingan
  - add -> commit
  - `git push -u origin main`
  - `git tag v1.0.0` nama tag untuk version pakai `v` depannya
  - `git push origin v1.0.0`

# Menambah Dependency
- Buat app-hello (step sama seperti sebelumnya)
- Di terminal: `go get github.com/FathanJundiR/go-hello-modules`

# Upgrade Module
Untuk upgrade module hanya dengan membuat tag baru.
Best practicenya tiap ada perubahan, dibikin tag baru walaupun minor.
- git commit push perubahan code di module
- `git tag v1.1.0`
- `git push origin v1.1.0` 

# Upgrade Dependency
- Ubah versinya di file `go.mod`
- `go get`

# Major Upgrade Module
Major upgrade biasanya yg breaking changes.
Biasanyav diganti nama module di go.mod dan tag version dinaikkan.
Before: github.com/FathanJundiR/go-hello-modules
After: github.com/FathanJundiR/go-hello-modules/v2

## Di go-hello
- Buat changes
- ganti isi go.mod `module github.com/FathanJundiR/go-hello-modules/v2`
- git add commit push
- `git tag v2.0.0`
- `git push origin v2.0.0`