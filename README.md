# Patika.dev-SQL-odev-4
Patika.dev &amp; FMSS İş Analisti Practicum SQL ödevi

<<code>
--ödev sorguları ms sql server üzerinden yazılmıştır.

--1.film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
select distinct replacement_cost from film;

--2.film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
select count(distinct replacement_cost) as 'Count' from film;

--3.film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
select count(*) as 'Count' from film where title like 'T%' and rating = 'G'

--4.country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
select count(*) as 'Count' from country where len(country)=5;

--5.city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
select count(*) from city where name like '%r' or name like '%R'
</code>>
