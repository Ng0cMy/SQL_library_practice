# SQL_library_practice

### We have 2 table:

#### 1. authors

|author_id|author_name|birth_year|
|---------|-----------|----------|
|1|Thich Nhat Hanh|1926|
|2|Stephen R.Covey|1932|
|3|Gian Tu Trung|1974|
|5|Jon Gordon|1971|
|6|Ohmae Kenichi|1943|

#### 2. books

|book_id|title|publication_year|author_id|
|-------|-----|----------------|---------|
|101|Phep la cua su tinh thuc|2023|1|
|102|7 thoi quen hieu qua|2018|2|
|103|Dung viec|2020|3|
|105|Tu duy ca map suy nghĩ ca vang|2017|5|
|106|Tu nay mam, tu vuon len|2012|6|

#### Data Integrity and Relations

SELECT author_name From authors WHERE author_id = (
SELECT author_id From books WHERE title = 'Phep la cua su tinh thuc');
