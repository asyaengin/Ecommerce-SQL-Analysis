--İlk 10 kayıt (veri yapısını görmek için)
SELECT * 
FROM satis_analizi
LIMIT 10;
-- Erkek müşterilerin tüm satış kayıtları
SELECT*
FROM satis_analizi
WHERE cinsiyet = 'Erkek';
--Giyim kategorisindeki tüm satışlar:
SELECT*
FROM satis_analizi
WHERE kategori = 'Giyim';
--Yaşı 30 ile 40 arasında olan müşteriler;
SELECT*
FROM satis_analizi
WHERE yas < 40 AND yas > 30 ;
--Yaşı 25'ten küçük olan müşteriler;
SELECT*
FROM satis_analizi
WHERE yas < 25;
--Satın alma tutarı 500 ile 1000 TL arasında olan satislar;
SELECT*
FROM satis_analizi
WHERE satin_alma_tutar > 20 AND satin_alma_tutar < 1000 
--Istanbul lokasyonundaki musterilerin listelenmesi;
SELECT*
FROM satis_analizi
WHERE lokasyon = 'İstanbul';
-- Mevsim olarak "yaz" ve "kış" olan satışlar;
SELECT*
FROM satis_analizi
where sezon IN ('Yaz','Kış');
