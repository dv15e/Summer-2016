# Summer-2016
grades=range(4);
i=0;
while True:
  try:	
		num = raw_input('Enter a number ')
		if num == "done" : 
			break
		grades[i]=num
		i=i+1
  except: 
  	  print "Invalid Input"
largest = grades[0];
smallest = grades[0];
print "How many grades inputed " , len(grades)
sum= 0
for grade in grades:
	if grade > largest:
		largest=grade
	if grade < smallest:
		smallest=grade
	print "the grades " , grade	
	sum = sum + int(grade)
average = sum / len(grades)
print "Maximum", largest
print "Minimum", smallest
print "Average", average
x = raw_input ("Enter number for grade: ")
if 90 <= int(x) <= 100:
	print "A"
elif 80 <= int(x) <= 89:
	print "B"
elif 70 <= int(x) <= 79:
	print "C"
elif 60 <= int(x) <= 69:
	print "D"
elif int(x) <= 59: 
	print "F"
print "All Done"
