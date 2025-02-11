# Working-with-cleaned-Data-Set-in-MySQL-from-Scratch

## ✏️ Question 1: Calculate the average review count for locations grouped by genre.
```SQL
SELECT genre, AVG(review_count) AS avg_review_count FROM ksa GROUP BY genre;
```
![image](https://github.com/user-attachments/assets/d1cc6246-7411-4adb-a81f-3e0520088f32)
