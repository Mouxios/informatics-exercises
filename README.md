# informatics-exercises
Ασκησεις πληροφορικης σε Excel, SQL, Python.

Εxcel
[excel τελικη.xlsx](https://github.com/user-attachments/files/20101654/excel.xlsx)

SQL
Μερικες λυσεις ασκησεων

1.
SELECT concat (Home_Team, "-", Away_Team) as matchup, 
concat (Home_Goals,"-", Away_Goals) as score
FROM reatcodeltd_axldp_QuarterFinals

2.
SELECT ID, FirstName, LastName, Age FROM maintable_PG4EI
where Lastname = "Smith" or Firstname = "Robert"
order by age

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

Python

