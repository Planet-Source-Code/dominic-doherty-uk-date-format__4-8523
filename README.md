<div align="center">

## uk date format


</div>

### Description

if when you want to use the date function and you do not want the continental style but the english then this code sorts it for you. very simple and easy to understand
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[dominic doherty](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dominic-doherty.md)
**Level**          |Beginner
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |ASP \(Active Server Pages\)
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__4-33.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dominic-doherty-uk-date-format__4-8523/archive/master.zip)





### Source Code

```
dim datetoday
'this is the variable that is made from the
'other three variables below. insert this
'variable in your code where you want the
'date to be displayed
dim nowday 'variable for today
dim nowmonth 'variable for current month
dim nowyear 'variable for current year
nowday =DatePart("D", Date) 'gets day number
nowmonth=DatePart("M", Date) 'gets month number
nowyear= DatePart("YYYY", Date) 'gets year
if nowday >=10 then
datetoday = nowday & "/" & nowmonth& "/"& nowyear
else nowday = "0" & nowday
'if the day number is less than 10 then a 0 is
'added infornt ie 8 goes to 08
end if
'the same is true below but for month number
if nowmonth >=10 then
datetoday = nowday & "/" & nowmonth& "/"& nowyear
else nowmonth = "0" & nowmonth
datetoday = nowday & "/" & nowmonth& "/"& nowyear
end if
'now you just insert the date where you want ie
response.write datetoday
'just trying to help beginners with small problems
hope it is helpful
```

