---
layout: post
title:  "Split String and Cast Date"
---

## Let's split a string variable and cast the date


```
$string = 'srv1 02-Dec-19'
$server,$strdate = $string.split(' ')
[datetime]$date = [datetime]::parseexact($strdate, 'dd-MMM-yy', $null).ToString('dd-MM-yyyy')
```   
