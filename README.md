# tableau_project
This is a tableau project where i have tried  to use most of the function in tableau on a data set to generate insights, prepare KPIs and Dashboards.
Few of the functions that i used are parameters, calculated field, sets, groups, also to for Dashboard i prepared a format in power point and uploaded it in tableau as image 
and placed my KPIs in it to make dashboard more attractive and professional.
To get YoY simply  create a calculated field and get corresponding value of present and previous year.
if YEAR([Issue D])={MAX(YEAR([Issue D]))} then ([Loan Amnt]) END 
if YEAR([Issue D])={MAX(YEAR([Issue D]))-1} then [Loan Amnt] END
for calculating mtd : current month value:  if DATEPART('year',[Issue D])={MAX(YEAR([Issue D]))} and DATEPART('month',[Issue D])={MAX(MONTH([Issue D]))} THEN [Loan Amnt] END
prevous monnth value: if DATEPART('year',[Issue D])={MAX(YEAR([Issue D]))} and DATEPART('month',[Issue D])={MAX(MONTH([Issue D]))}-1 THEN [Loan Amnt] END
now we can use this to calculate MoM increment.
Also to make it interactive with the user we can create Parameter to show top n values where value will be a input from user.
we combine this parameter with set to make it functionqal and dynamic.
To make the symbol  dynamic with the value you can use caluculayed field with formula: IF [YOY LOAN AMNT]>=0 THEN "▲" ELSE "▼" END
To prepare dashboard i have prepared a format using power point and uploaded it as image in dashboard page and placed my visuals in it.
