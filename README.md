# Awake

macOS menü çubuğunda çalışan küçük bir uygulama. İki şey yapar, ikisi de ayrı ayrı süreli ya da sonsuz çalışır:

- **Kapak Kapalı** — MacBook'un kapağı kapalıyken bile uykuya geçmesini engeller.
- **Uyanık Tut** — Mac'in boşta kalınca uykuya geçmesini engeller (Theine / Amphetamine gibi).

Tanıtım ve indirme: https://berkehankucukaras.github.io/awake/

## Kurulum

1. [Releases](../../releases) sayfasından `Awake.dmg` dosyasını indirip açın.
2. Açılan pencerede **Awake**'i **Applications** klasörüne sürükleyin ve Uygulamalar'dan açın. Uygulama menü çubuğunda bir laptop simgesi olarak görünür; ayrıca girişte otomatik başlar.
3. **Kapak Kapalı** özelliğini ilk kez açtığınızda macOS bir kez yönetici parolası sorar. Bu, yalnızca iki `pmset` komutu için `/etc/sudoers.d/awake` dosyasına parolasız izin yazar; sonraki açma-kapamalarda parola sorulmaz. **Uyanık Tut** hiç parola istemez.

Uygulama Developer ID ile imzalı ve Apple tarafından noterlenmiştir. macOS 13 ve üzeri, Apple Silicon ve Intel.

Kaldırmak için uygulamayı silmek yeterli; isterseniz `sudo rm /etc/sudoers.d/awake` ile izni de kaldırın.

## Uyarı

"Kapak Kapalı" açıkken Mac'i kapağı kapalı hâlde çantaya koyarsanız uyanık kalır ve ısınabilir. Uygulamadan çıkarken açık olan özellikler kendiliğinden kapatılır.

## Geri bildirim

Hata ve öneriler için [Issues](../../issues) sayfasını kullanın.
