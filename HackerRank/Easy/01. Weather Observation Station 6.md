# 문제 1. Weather Observation Station 6

Q. Query the list of CITY names starting with vowels (i.e., a, e, i, o, or u) from STATION. <br>
Your result cannot contain duplicates.

🔑 문제 풀이
```mysql
SELECT DISTINCT CITY
FROM STATION 
WHERE CITY REGEXP '^[aeiou].*'
```

출처: [HackerRank 문제 보기](https://www.hackerrank.com/challenges/weather-observation-station-6/problem?isFullScreen=true)

-----

#### 💡 ^ Beginning: Matches the beginning of the string.
#### 💡 [] Character set: Match any character in the set. 
#### 💡 . Dot: Matches any character except line breaks.
#### 💡 * Quantifier: Match 0 or more of the preceding token.
