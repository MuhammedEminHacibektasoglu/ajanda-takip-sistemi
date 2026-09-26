# Proje: Günlük Ajanda Takip Sistemi

## Proje Tanımı
Kullanıcıların günlük görevlerini eklediği, tamamlanma durumunu işaretlediği ve
hatırlatıcı ayarladığı bir web uygulaması. Ders projesi kapsamında geliştiriliyor.

## Teknik Kararlar
- Dil: Vanilla PHP (framework yok) + PDO
- Veritabanı: MySQL
- Ortam: Laragon (lokal), hosting henüz seçilmedi
- Versiyon kontrolü: Git + GitHub
  - Repo: https://github.com/MuhammedEminHacibektasoglu/ajanda-takip-sistemi

## Şu Anki Durum (Son güncelleme: 26 Eylül 2026)
- [x] Lokal sunucu ortamı kuruldu (Laragon, PHP 8.3.33, MySQL)
- [x] phpMyAdmin erişimi sağlandı
- [x] VS Code + PHP eklentileri kuruldu (Intelephense, PHP Debug, SQLTools, GitLens, Error Lens)
- [x] `ajanda_db` veritabanı oluşturuldu (henüz tablo yok)
- [x] Git + GitHub bağlantısı kuruldu, ilk commit'ler atıldı
- [x] Claude Code CLI + VS Code eklentisi kuruldu
- [x] `index.php`'deki `phpinfo()` test satırı kaldırıldı ve GitHub'a push edildi (commit `c6ef9bf`)
- [ ] `.gitignore` henüz boş; DB bağlantı dosyası eklenmeden önce kurallar yazılmalı
- [ ] Veritabanı tabloları henüz tasarlanmadı (users, tasks, reminders)
- [ ] Kullanıcı kayıt/giriş sistemi yazılmadı
- [ ] Görev ekleme/listeleme/tamamlama yazılmadı
- [ ] Hatırlatıcı sistemi yazılmadı
- [ ] Admin paneli yazılmadı

## Sıradaki Adım
Veritabanı şemasını tasarlamak: users, tasks, reminders tabloları.

## Dikkat Edilecekler
- `phpinfo()` gibi debug amaçlı kodlar production'a gitmeden önce silinmeli
- Şifreler ve DB bağlantı bilgileri `.gitignore` ile GitHub'a gitmemeli
- Hocanın istediği 2 haftada bir PDF rapor teslimini unutma (en az 2 sayfa)
- Tüm SQL sorgularında PDO prepared statement kullanılacak (SQL injection'a karşı)

## Çalışma Alışkanlığı
- Her oturum sonunda bu dosyayı güncel ilerlemeye göre güncelle
- Anlamlı commit mesajları yaz (rapor yazarken işine yarayacak)
