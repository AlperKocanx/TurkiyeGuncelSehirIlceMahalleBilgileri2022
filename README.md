# TurkiyeGuncelSehirIlceMahalleBilgileri2022
Türkiye'nin güncel İl, İlçe ve mahalle bilgilerinin yer aldığı SQL dosyasıdır. İlçe ve Mahallelerin koodinat bilgilerini de içerir.

SQL veritabanınıza kolaylıkla ekleyebilir, sonrasında istediğiniz düzenlemeleri yapabilirsiniz.

MySQL için yeni eklenmiş CSV dosyasını kullanabilirsiniz.

UstID sütunu '0' olan kayıtlar illeri, UstID bilgisi sıfırdan farklı olan veriler ise ilgili UstID'ye bağlı birimi gösterir.

Örneğin,

select * from YeniAdresTablosu where ID = 6 or ID = 1132 or ID = 6804 sorgusu ile, ANKARA İline bağlı YENİMAHALLE ilçesine bağlı 25 MART mahallesine erişilir.

(UstID'si 6 olan tüm kayıtlar ANKARA iline bağlı ilçeler, UstID'si 1132 olan tüm kayıtlar YENİMAHALLE ilçesine bağlı mahallelerdir.)

![image](https://user-images.githubusercontent.com/47237365/192288710-783e7523-b510-4d2a-8059-01ecf3a401f9.png)


Veriler güncel olup, ara ara güncelliği için ilgili dosya değiştirilecektir. (58.158 kayıt)

Son Güncelleme tarihi : 26.09.2022
