1) ********** # R **********
# Input Section
Employee_Name <- readline('Employee Name : ' )
Employee_ID <- readline('Emp Id : ')
Employee_Salary_Monthly <- as.integer(readline('Monthly Salary : '))
Leave_Days <- as.integer(readline('Leave Days : '))
TDS_Percentage <- 2
Month <- as.integer(readline('Month : '))
Year <- 2023

# Calculations
Yearly_Salary <- (Employee_Salary_Monthly * 12)
Leave_Amount <- (Employee_Salary_Monthly / 30) * Leave_Days
TDS_Amount <- (Employee_Salary_Monthly * TDS_Percentage) / 100
Final_Pay_Salary <- Employee_Salary_Monthly - Leave_Amount - TDS_Amount

# Output Section
# cat("Name:", Employee_Name, "\n")
# cat("EMP ID:", Employee_ID, "\n")
# cat("Monthly Salary:", Employee_Salary_Monthly, "/-\n")
cat("CTC (Yearly Salary):", Yearly_Salary, "/-\n")
cat("Leave Amount:", Leave_Amount, "/-\n")
cat("TDS Amount:", TDS_Amount, "/-\n")
cat("Final Pay Salary:", Final_Pay_Salary, "/-\n")
cat("Date:", month.name[Month], "/", Year)


2) ********** # function with return type arg.. **********
tax <- function(price,gst){
  gst <- price*gst/100
  price <- gst+price
  return(price)
}
cat('Mrp = ',tax(1200,12))

3) ********** # function with arg... **********

result <- function(number1,number2){
  add = number1+number2
  cat('This is result : ',add)
}
# calling function
result(25,25)

4)********** # Example: Using a repeat loop to count from 1 to 10 **********

count <- 1

repeat {
  cat('count: ',count, '\n')
  count <- count+1
  if(count > 10)
  break # Terminate the loop when count reaches 10
}

5) ********** # R ifelse() function **********
# ifelse('test_expression, Yes_expression, No_expression')
a = 20
b = 30
ifelse( a < b, 'a is smallest','a is not smallest')






# ********** vectorized operations **********
numeric_vector <- c(1,2,3,4,5)
squer_vector <- numeric_vector^2
squer_vector

qube_vector <- numeric_vector^3
qube_vector
