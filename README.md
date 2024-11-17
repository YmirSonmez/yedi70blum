
---

## Kullanım Öncesi Öneriler

# 🔥🔥 PYTHON sürümü 3.10 olmalıdır 🔥🔥

> 🇷 🇺 Rusça README [burada](README-RU.md) mevcuttur.

## Özellikler  
|                      Özellik                      | Destekleniyor |
|:-------------------------------------------------:|:-------------:|
|                   Çoklu iş parçacığı (Multithreading) |     ✅     |
|              Proxy'yi oturumla bağlama               |     ✅     |
| Hesabınızı referans linkinizle otomatik kaydetme     |     ✅     |
|      Rastgele puan seçimiyle otomatik oyun oynama    |     ✅     |
|           pyrogram .session desteği                |     ✅     |

## [Ayarlar](https://github.com/YmirSonmez/yedi70blum/blob/main/.env-example/)
|              Ayarlar                |                                 Açıklama                                   |
|:-----------------------------------:|:----------------------------------------------------------------------------:|
|        **API_ID / API_HASH**        |   Telegram oturumu için platform verileri (varsayılan - android)            |
|           **PLAY_GAMES**            |              Oyun oynatmak ya da sadece çiftçilik yapmak (varsayılan: True) |
|             **POINTS**              |        Oyundaki puanlar (varsayılan: [190, 230] yani 190 ile 230 arasında)  |
|           **AUTO_TASKS**            |                      Görevleri yap ya da yapma (varsayılan: True)          |
|         **TRIBE_CHAT_TAG**          |                    Otomatik katılım için kabile telegram etiketiniz        |
|     **USE_RANDOM_DELAY_IN_RUN**     |                              Kendisi ismini açıklar                        |
|       **RANDOM_DELAY_IN_RUN**       |               Rastgele saniye gecikmesi için yukarıdaki ayar (varsayılan: [5, 30]) |
|             **USE_REF**             |         Hesapları referans linkinizle kaydeder mi? (varsayılan - False)     |
|             **REF_ID**              |  Referans kimliğiniz (app/startapp? sonrasındaki parametre: _r_abcde1234_) |
|       **USE_PROXY_FROM_FILE**       | `bot/config/proxies.txt` dosyasından proxy kullanıp kullanmayacağı (True / False) |
| **SLEEP_MINUTES_BEFORE_ITERATIONS** |  Kontroller arasındaki bekleme süresi (varsayılan: [120, 600] yani 120 ile 600 dakika arası) |
|              **DEBUG**              |          Rastgele gecikmeyi devre dışı bırakır ve log seviyesini DEBUG yapar |

## Hızlı Başlangıç 📚

Kütüphaneleri hızlı bir şekilde yükleyip botu çalıştırmak için Windows'ta `run.bat` dosyasını ya da Linux'ta `run.sh` dosyasını açın.

## Ön Gereksinimler
Başlamadan önce aşağıdaki yazılımların yüklü olduğundan emin olun:
- [Python](https://www.python.org/downloads/) **sürüm 3.10**

## API Anahtarlarını Alma
1. my.telegram.org adresine gidin ve telefon numaranızla giriş yapın.
2. "API geliştirme araçları"nı seçin ve yeni bir uygulama kaydetmek için formu doldurun.
3. Uygulamanızı kaydettikten sonra verilen **API_ID** ve **API_HASH**'i `.env` dosyasına kaydedin.

## Kurulum
**[Depoyu](https://github.com/YmirSonmez/yedi70blum)** sisteminize klonlayarak gerekli bağımlılıkları yükleyebilirsiniz:
```shell
git clone https://github.com/YmirSonmez/yedi70blum.git
cd yedi70blum
```

Ardından, otomatik kurulum için şunları yazabilirsiniz:

Windows:
```shell
run.bat
```

Linux:
```shell
run.sh
```

# Linux Manual Kurulumu
```shell
sudo sh install.sh
python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt
cp .env-example .env
nano .env  # Burada API_ID ve API_HASH'inizi belirtmeniz gerekmektedir, geri kalan varsayılan olarak alınır.
python3 main.py
```

Ayrıca hızlı başlatma için komut satırı argümanları da kullanabilirsiniz:
```shell
~/BlumTelegramBot >>> python3 main.py --action (1/2)
# Ya da
~/BlumTelegramBot >>> python3 main.py -a (1/2)

# 1 - Tıklayıcıyı çalıştır
# 2 - Bir oturum oluştur
```

# Windows Manual Kurulumu
```shell
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
copy .env-example .env
# Burada API_ID ve API_HASH'inizi belirtmeniz gerekmektedir, geri kalan varsayılan olarak alınır.
python main.py
```

Ayrıca hızlı başlatma için komut satırı argümanları da kullanabilirsiniz:
```shell
~/BlumTelegramBot >>> python main.py --action (1/2)
# Ya da
~/BlumTelegramBot >>> python main.py -a (1/2)

# 1 - Tıklayıcıyı çalıştır
# 2 - Bir oturum oluştur
```

---
