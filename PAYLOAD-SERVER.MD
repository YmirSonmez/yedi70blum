
# Payload Generator

Ne için gereklidir? Blum güncellemeleri nedeniyle, oyun sonucunun doğrulanma algoritması değiştirildi. Oyunu bitirmek için, faydalı yükün karmaşık bir değeri hesaplanmalıdır, ancak bu algoritmayı basit bir şekilde bota entegre etmek mümkün değildir. Ancak geliştirici **[sanjithacks](https://github.com/sanjithacks)**, oyun uygulamasından jeneratörü çıkarıp sonuçlarını **[flower-signer](https://github.com/sanjithacks/flower-signer)** deposunda paylaştı.  
Başka bir geliştirici **[Arthur Koba](https://github.com/ArthurKoba)**, bu çalışmaları kullanarak **[faydalı yük üretim sunucusu](https://github.com/KobaProduction/BlumPayloadGenerator)** oluşturdu. Bu sunucu, çalıştırılabilir ve herhangi bir programlama dilinde kullanılabilir çünkü REST API üzerinden iletişim sağlar.

# Kullanım Bilgisi

1. Node.js'i yüklemeniz gerekmektedir (veya güncellemeniz, 20 ve üstü sürüm gereklidir).
2. [Faydalı Yük Üretim Sunucusunu](https://github.com/KobaProduction/BlumPayloadGenerator) yükleyin.
3. Sunucuyu çalıştırın ve kapatmayın! Sunucu sürekli çalışmalı ve aynı anda botla birlikte açık olmalıdır.  
   ###### **Bunu nasıl yapacağınızı bilmiyorsanız - lütfen bana (Arthur Koba) mesaj atmayın ve depo üzerinde sorun açmayın.**  
   ###### **Bu sorun geliştiricilerle değil, tamamen sizinle ilgilidir. Kendi başınıza çözüm bulmaya çalışın veya [Hidden Code sohbetine](https://t.me/hidden_codding_chat/16053) yazın.**

# Özellikler ve Neden Böyle Yapıldı

1. Bot yerel olarak kullanılabilir, başka sunuculara bağımlı değildir. Daha önce bot, dış sunuculardan faydalı yük alarak oyun oynuyordu, ancak bu sunucuların sahibi ödeme talep etti, bu da botun çalışmasını bozdu. Bu tür sorunlarla karşılaşmamak için, jeneratör yerel olarak kullanılabilir ve kimseye ödeme yapmanıza gerek kalmaz.
2. Ayrıca faydalı yük sunucusunu bir hosting üzerinde çalıştırma imkanınız vardır ve bota dış IP adresini verebilirsiniz. Bu durumda da bot çalışacaktır. Bunu nasıl yapacağınızı? Yine, kendi başınıza çözüm bulmaya çalışın veya size yardımcı olacak birini bulun.
3. Botun başka sunucularla uyumluluğu sağlanmamıştır, bu konu tartışılmamaktadır.

--- 

Bu çeviri metnin içeriğini doğru bir şekilde Türkçeye aktarır. Yardımcı olabileceğim başka bir konu varsa, lütfen belirtin!