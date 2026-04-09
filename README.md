У процесі виконання роботи було закріплено навички роботи з SQL-запитами. Зокрема, використано оператори для вибірки даних, фільтрації, сортування та обмеження результатів. Також застосовано агрегатні функції для аналізу даних і групування записів.

Робота дозволила краще зрозуміти структуру бази даних та принципи роботи з реальними даними, імпортованими з CSV-файлів.
SELECT name, phone FROM shippers;

SELECT 
    AVG(price), MAX(price), MIN(price)
FROM products;

SELECT DISTINCT category_id, price
FROM products
ORDER BY price DESC
LIMIT 10;

SELECT COUNT(*)
FROM products
WHERE price BETWEEN 20 AND 100;

SELECT 
    supplier_id,
    COUNT(*),
    AVG(price)
FROM products
GROUP BY supplier_id;
SELECT * FROM products;
