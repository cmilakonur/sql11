# sql11
patika.dev linkim: https://app.patika.dev/cmilakonur <br />

1- actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım. <br />
select first_name <br />
from actor <br />
union <br />
select first_name <br />
from customer <br />

2- actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım. <br />
select first_name <br />
from actor <br />
intersect <br />
select first_name <br />
from customer <br />

3- actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım. <br />
select first_name  <br />
from actor <br />
except  <br />
select first_name <br />
from customer <br />

4- İlk 3 sorguyu tekrar eden veriler için de yapalım. <br />
* select first_name from actor <br />
  UNION ALL <br />
  select first_name from customer <br />

* select first_name from actor <br />
  INTERSECT ALL <br />
  select first_name from customer <br />

* select first_name from actor <br />
  EXCEPT ALL <br />
  select first_name from customer <br />
