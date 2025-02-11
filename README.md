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



