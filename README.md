# sqlodev4
 sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1-)film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
select DISTINCT replacement_cost FROM film;
2-)film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
select COUNT(DISTINCT replacement_cost) from film;
3-)film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
select COUNT (title) from film where title LIKE('T%') AND rating = 'G';
4-)country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
select COUNT (country) from country where country LIKE('%%%%%');
5-)city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
select COUNT (city) from city where city ILIKE('%r);
