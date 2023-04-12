# Patika.dev-SQL-odev-4
Patika.dev &amp; FMSS İş Analisti Practicum SQL ödevi

### ödev sorguları ms sql server üzerinden yazılmıştır.

##### 1.film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
<<code> select distinct replacement_cost from film; </code>>

##### 2.film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
<<code> select count(distinct replacement_cost) as 'Count' from film; </code>>

##### 3.film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
<<code> select count(*) as 'Count' from film where title like 'T%' and rating = 'G' </code>>

##### 4.country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
<<code> select count(*) as 'Count' from country where len(country)=5; </code>>


##### 5.city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
<<code> select count(*) from city where name like '%r' or name like '%R' </code>>
