# 🧑‍💻 Working-with-cleaned-Data-Set-in-MySQL-from-Scratch

## ✏️ Question 1: Calculate the average review count for locations grouped by genre.
```SQL
SELECT genre, AVG(review_count) AS avg_review_count FROM ksa GROUP BY genre;
```
![image](https://github.com/user-attachments/assets/d1cc6246-7411-4adb-a81f-3e0520088f32)


## ✏️ Question 2: Retrieve all rows where the rating is 5.
```sql
SELECT * FROM ksa WHERE rating = 5;
```
![image](https://github.com/user-attachments/assets/3cfc650f-4450-4b7b-88f4-875b0af5a449)

## ✏️ Question 3: List the names of locations with over 10,000 reviews.
```sql
SELECT name FROM ksa WHERE review_count > 10000;
```
![image](https://github.com/user-attachments/assets/caa00820-6b93-4875-b4e8-7f72aa0031bd)

## ✏️ Question 4: Find the total number of locations with a rating of 0.
```sql
SELECT COUNT(*) AS count_rating_zero FROM ksa WHERE rating = 0;
```
![image](https://github.com/user-attachments/assets/cc587e37-8508-43cd-bec0-44f0cd140e72)

## ✏️ Question 5: Find the average rating across all locations.
```sql
SELECT AVG(rating) AS average_rating FROM ksa;
```
![image](https://github.com/user-attachments/assets/0824ca4b-fc19-4ab3-b83e-7c7668efe600)

## ✏️ Question 6: What are the top 5 locations based on rating and number of reviews?
```sql
SELECT name, rating, review_count 
FROM ksa 
ORDER BY rating DESC, review_count DESC 
LIMIT 5
```
![image](https://github.com/user-attachments/assets/1fd5c7df-5fc4-4d0e-8b73-05f3ae5f1657)

## ✏️ Question 7: What are the locations with a rating below 3 and more than 10,000 reviews?
```sql
SELECT name, rating, review_count 
FROM ksa 
WHERE rating < 3 AND review_count > 10000;
```
![image](https://github.com/user-attachments/assets/ace95949-93b9-4308-9882-2ddadcabb39b)

## ✏️ Question 8: How can we display all the information about every location in the dataset?
```sql
SELECT * FROM ksa;
```
![image](https://github.com/user-attachments/assets/4af522b8-c1d3-4ce8-9f32-dcb28e07c3d3)

## ✏️ Question 9: How can we list all unique genres available in the dataset?
```sql
SELECT DISTINCT genre FROM ksa;
```
![image](https://github.com/user-attachments/assets/3e73e810-bb2e-4a54-806d-3212d8e50534)

## ✏️ Question 10: How can we find the names of locations in Khobar?
```sql
SELECT name FROM ksa WHERE location LIKE '%Khobar%';
```
![image](https://github.com/user-attachments/assets/d190ea2b-782a-481a-a6c7-1fb799ce7564)





















