-- 1
SELECT * FROM startups;

--2
SELECT COUNT(*) AS 'Total number of companies' FROM startups;

--3
SELECT SUM(valuation) AS 'Total value of all companies' FROM startups;

--4
SELECT MAX(raised) AS 'Max amount raised by a startup' FROM startups;

--5
SELECT MAX(raised) AS 'Max amoumt of money during Seed stage' FROM startups
WHERE stage = 'Seed';

--6
SELECT MIN(founded) AS 'The year the oldest company founded' FROM startups;

-- 7
SELECT AVG(valuation) AS 'Average valuation' FROM startups;

-- 8
SELECT category, AVG(valuation) AS 'Average valuation' FROM startups
GROUP BY category;

-- 9
SELECT category, ROUND(AVG(valuation), 2) AS 'Rounded average valuation' FROM startups
GROUP BY category;

-- 10
SELECT category, ROUND(AVG(valuation), 2) AS 'Rounded and sorted average valuation' FROM startups
GROUP BY 1
ORDER BY 2 DESC;

-- 11
SELECT category, COUNT(*) as 'Number of companies' FROM startups
GROUP BY category;

--12
SELECT category, COUNT(*) as 'Number of companies (> 3)' FROM startups
GROUP BY category
HAVING COUNT(*) > 3;

-- 13
SELECT location, AVG(employees) AS 'Average size' FROM startups
GROUP BY location;

-- 14
SELECT location, AVG(employees) AS 'Average size of startup' FROM startups
GROUP BY location
HAVING AVG(employees) > 500;