# SQL-ODEV-5
film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.
ÇÖZÜM: SELECT* FROM film
WHERE title LIKE '%n'
ORDER BY length
LIMIT 5

![1231321](https://user-images.githubusercontent.com/128131203/226562300-ff54ac61-e3cf-4225-bcab-7bb9c746649a.PNG)

film tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci(6,7,8,9,10) 5 filmi(6,7,8,9,10) sıralayınız.
ÇÖZÜM: SELECT* FROM film
WHERE title LIKE '%n'
ORDER BY length ASC
OFFSET 1
LIMIT 5

![546546](https://user-images.githubusercontent.com/128131203/226563207-5d121b6a-b78b-4c8c-ac5a-22ee67a4d0f4.PNG)

customer tablosunda bulunan last_name sütununa göre azalan yapılan sıralamada store_id 1 olmak koşuluyla ilk 4 veriyi sıralayınız.
ÇÖZÜM: SELECT* FROM Customer
WHERE store_id= 1
ORDER BY last_name DESC
LIMIT 4

![456564](https://user-images.githubusercontent.com/128131203/226563742-c2af57d1-f907-4a8f-990d-74b3ea703627.PNG)
