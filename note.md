- Buat repository baru di github
- Buat modules di local:
  - Bikin folder baru
  - `go mod init URL_repo_github`
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
- Di terminal: `go get nama_module`
