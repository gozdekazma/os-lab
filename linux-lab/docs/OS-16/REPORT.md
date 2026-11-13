# OS-16 — Sunucuya ilk bakış raporu

**Öğrenci:** Gözde Kazma (@gozdekazma)  
**Ders:** MYO203 — Açık Kaynak İşletim Sistemleri  
**Rezervasyon:** [#113](https://github.com/keyvanarasteh/os-lab/pull/113)

## Yapılan çalışma

`server_firstlook.py`, Linux sunucusuna ilk girişte gereken bilgileri tek
çalıştırmada toplar. `uname`, `lsb_release`, `inxi`, `free`, `df` ve `systemctl`
çıktılarından okunabilir metin ve JSON üretir. Mimari notu, `x86_64` ile `amd64`
gibi farklı adların paket seçimindeki anlamını açıklar. Kod yalnızca Python
standart kütüphanesini kullanır.

Komut bulunamadığında veya systemd çalışmadığında rapor diğer bölümlerle devam
eder; eksik veri açıkça işaretlenir. Her komuta zaman sınırı uygulanır. Araç
paket kurmaz, servis başlatıp durdurmaz ve ağdaki başka sistemlere bağlanmaz.
Otomatik testler hem başarılı hem hatalı komut çıktılarıyla davranışı kontrol eder.

## Git ve PR akışındaki kavramlar

- Fork, ana projenin GitHub hesabındaki kopyasıdır; clone çalışma ortamına indirir.
- `feat/server-firstlook` dalı, bu görevi ana daldan ayrı geliştirir.
- Commit değişikliklerin kayıt noktasıdır; push commit'leri uzak dala gönderir.
- Pull Request, değişikliğin hocanın deposuna alınmasını isteyen inceleme kaydıdır.
- Rezervasyon PR'ı ile çalışan uygulamanın PR'ı farklı amaçlara hizmet eder.
- Aynı dala yeni commit gönderildiğinde açık PR güncellenir; tekrar PR açılmaz.

## Destek ve kalan öğrenci doğrulaması

Kod, testler ve belge taslağı ChatGPT desteğiyle hazırlanmıştır. Bu bölüm kişisel
öğrenme beyanı yerine geçmez. Gözde kendi labında çalıştırdıktan sonra aşağıdaki
alanları kendi deneyimine göre tamamlamalı ve metni gözden geçirmelidir:

- Kullandığım Linux dağıtımı ve mimarisi: **henüz kaydedilmedi**.
- Çalıştırmada gözlemlediğim sonuç / karşılaştığım sorun: **henüz kaydedilmedi**.
- Git/PR sürecinde öğrendiğim şey ve bunu nasıl kullandığım: **henüz yazılmadı**.
- 2–4 dakikalık kanıt videosu: **henüz eklenmedi**.

Tekrar çalıştırma komutları ve video sırası [VERIFY.md](VERIFY.md) içindedir.
