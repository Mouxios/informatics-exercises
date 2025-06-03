# informatics-exercises

Εxcel
[excel τελικη.xlsx](https://github.com/user-attachments/files/20101654/excel.xlsx)

SQL

1.
SELECT concat (Home_Team, "-", Away_Team) as matchup, 
concat (Home_Goals,"-", Away_Goals) as score
FROM reatcodeltd_axldp_QuarterFinals;

2.
SELECT ID, FirstName, LastName, Age FROM maintable_PG4EI
where Lastname = "Smith" or Firstname = "Robert"
order by age;

3.
select store_name, count(distinct item_number) as item_count
FROM reatcodeltd_axldp_finance
group by store_name
order by store_name;

4.
SELECT city, MAX(state_bottle_cost) as highest_cost, MIN(state_bottle_cost) as lowest_cost
FROM reatcodeltd_axldp_finance
group by city
order by city;

5.
SELECT LastName, Sum(Age) as SumAge
FROM maintable_5Y69Y
where LastName = "Smith"
group by LastName ;

6.
SELECT city, population FROM north_american_cities
WHERE country LIKE "United States"
ORDER BY population DESC
LIMIT 2 OFFSET 2;

7.
SELECT title FROM movies
ORDER BY title ASC
LIMIT 5 OFFSET 5;

8.
SELECT customer_id, SUM(amount) AS total_amount
FROM orders
GROUP BY customer_id;

9.
SELECT customers.name, SUM(orders.amount) AS total_amount
FROM customers
JOIN orders ON customers.customer_id = orders.customer_id
GROUP BY customers.name;

PYTHON

1.
def SimpleAdding(num):
    x = 0
    for i in range(0, num + 1):
        x = x + i
    return x
print(SimpleAdding(int(input())))

2.
def CheckNums(num1, num2):
    if num1 < num2:
        x = "True"
    elif num1 == num2:
        x = -1
    else:
        x = "False"
    return x
  print(CheckNums(input()))

  3.
  def Division(num1, num2):
    high = 1
    if num1 >= num2:
        size = num1
    else:
        size = num2
    for x in range(1, size):
        if (num1 % x == 0) and (num2 % x == 0) and (x > high):
            high = x
    return high
print(Division(int(input()), int(input())))
