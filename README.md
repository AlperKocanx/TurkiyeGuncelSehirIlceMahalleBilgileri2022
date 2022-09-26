# TurkiyeGuncelSehirIlceMahalleBilgileri2022
Türkiye'nin güncel İl, İlçe ve mahalle bilgilerinin yer aldığı SQL dosyasıdır. İlçe ve Mahallelerin koodinat bilgilerini de içerir.

SQL veritabanınıza kolaylıkla ekleyebilir, sonrasında istediğiniz düzenlemeleri yapabilirsiniz.

UstID sütunu '0' olan kayıtlar illeri, UstID bilgisi sıfırdan farklı olan veriler ise ilgili UstID'ye bağlı birimi gösterir.

Örneğin,

select * from YeniAdresTablosu where ID = 6 or ID = 1132 or ID = 6804 sorgusu ile, ANKARA İline bağlı YENİMAHALLE ilçesine bağlı 25 MART mahallesine erişilir.

(UstID'si 6 olan tüm kayıtlar ANKARA iline bağlı ilçeler, UstID'si 1132 olan tüm kayıtlar YENİMAHALLE ilçesine bağlı mahallelerdir.)


ID	  SehirIlceMahalleAdi	  UstID	  minlongitude	  minlatitude	  maxlongitude	  maxlatitude	  MahalleID
6	    ANKARA	                0	      NULL	            NULL	        NULL	          NULL	      NULL
1132	YENİMAHALLE	            6	    32.563202	      39.91101	    32.847119	      40.104982	      1723
6804	25 MART (MERKEZ)	    1132	  32.79013	      39.950773	    32.801409	      39.958041	      NULL


Veriler güncel olup, ara ara güncelliği için ilgili dosya değiştirilecektir.

Son Güncelleme tarihi : 26.09.2022
