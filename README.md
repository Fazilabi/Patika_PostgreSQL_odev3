# Patika_PostgreSQL_odev3
## [Patika.dev](www.patika.dev)

## 1. country tablosunda bulunan country sütunundaki ülke isimlerinden 'A' karakteri ile başlayıp 'a' karakteri ile sonlananları sıralayınız.<br>
SELECT country  FROM country <br>
WHERE country LIKE 'A%a';

## 2. country tablosunda bulunan country sütunundaki ülke isimlerinden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
SELECT country  FROM country <br>
WHERE country LIKE '_____%n';

## 3. film tablosunda bulunan title sütunundaki film isimlerinden en az 4 adet büyük ya da küçük harf farketmesizin 'T' karakteri içeren film isimlerini sıralayınız.
SELECT title FROM film <br>
WHERE title  ILIKE '%t%t%t%t';

## 4. film tablosunda bulunan tüm sütunlardaki verilerden title 'C' karakteri ile başlayan ve uzunluğu (length) 90 dan büyük olan ve rental_rate 2.99 olan verileri sıralayınız.
SELECT * FROM film <br>
WHERE title LIKE 'C%' <br>
AND length > 90 <br>
AND RENTAL_RATE  = 2.99;
