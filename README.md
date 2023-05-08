Download Link: https://assignmentchef.com/product/solved-solved-a4-solved
<br>
Modify the Time class of Figs. 9.4–9.5(attached) to be able to work with Date class. The Time object should always remain in a consistent state.

Modify the Date class of Figs. 9.17- 9.18(attached) to include a Time class object as a composition, a tick member function that increments the time stored in a Date object by one second, and increaseADay function to increase day, month and year when it is proper. Please use CISP400V9A4.cpp that tests the tick member function in a loop that prints the time in standard format during iteration of the loop to illustrate that the tick member function works correctly. Be aware that we are testing the following cases:

a) Incrementing into the next minute.

b) Incrementing into the next hour.

c) Incrementing into the next day (i.e., 11:59:59 PM to 12:00:00 AM).

d) Incrementing into the next month and next year.

Time class

The Time class has three private integer data members, hour (0 – 23 (24-hour clock format)), minute (0 – 59), and second (0 – 59).

It also has Time, setTime, setHour, setMinute, setSecond, getHour(), getMinute, getSecond,~Time, printUniversal, and printStandard public functions.

The Time function is a default constructor. It takes three integers and they all have 0 as default values. It also displays “Time object constructor is called.” message and calls printStandard and printUniversal functions.The setTime function takes three integers but does not return any value. It initializes the private data members’ (hour, minute and second) data.The setHour function takes one integer but doesn’t return anything. It validates and stores the integer to the hour private data member.The setMinute function takes one integer but doesn’t return anything. It validates and stores the integer to the minute private data member.The setSecond function takes one integer but doesn’t return anything. It validates and stores the integer to the second private data member.The getHour constant function returns one integer but doesn’t take anything. It returns the private data member hour’s data.The getMinute constant function returns one integer but doesn’t take anything. It returns the private data member minute’s data.The getSecond constant function returns one integer but doesn’t take anything. It returns the private data member second’s data.The Time destructor does not take anything. It displays “Time object destructor is called.” message and calls printStandard and printUniversal functions.The printUniversal constant function does not return or accept anything. It displays time in universal-time format.The printStandard constant function does not return or accept anything. It displays time in standard-time format.

Date class

The Date class has three private integer data members (month, day and year), one private Time object (time) data member and one static constant integer variable (monthsPerYear).

It has Date, print, increaseADay, tick, and ~Date public functions. It has one private checkDay function.

1. The Date function is a default constructor. It takes 3 integers and one Time object. The three integers have default data (1, 2, and 1900) and the Time has (0, 0, and 0) as default data. It displays “Date object constructor for date” information when the constructor is called.

2. The print constant function does not take or return data. It prints out the month day year, hour, minute and second information.

3. The increaseADay function does not take or return data. It increases the private data member day by one. It also checks the day to make sure the data is accurate. If the data is not accurate it will adjust all the necessary corresponding data.

4. The tick function does not takes or return data. It increases one second to the Time object of the Date class private data member. This function has to make sure that the second increased is proper or it will adjust all the necessary corresponding data.

5. The ~Date function is a destructor of the Date class. It also displays “Date object destructor is called “; message and calls Time object destructor.

6. The constant checkDay function takes and returns an integer. It makes sure the accuracy of day, month, and year information. This utility function to confirm proper day value based on month and year, it also handles leap years, too.

This assignment comes with a CISP400V9A4.zip file. It includes six files (CISP400V9A4.cpp, CISP400V9A4.exe, Date.cpp, Date.h, Time.cpp and Time.h). The CISP400V9A4.exe file is an executable file. You can double click the file to get to the expecting result (see the picture below) of this assignment. The Date.cpp, Date.h, Time.cpp, and Time.h are files coming from the textbook examples which you can use so you don’t need to start from scratch. After you finish your implementation for the Date and Time class, you can put the CISP400V9A4.cpp, Date.cpp, Date.h, Time.cpp, and Time.h in a project and then you can run to the same result as the CISP400V9A4.exe. Please be awarded that you can adjust only your program (Date.cpp, Date.h, Time.cpp and Time.h) to generate the required result but not the code in CISP400V9A4.cpp file.

The following are the couple displays of the expecting results.

The picture in the next column is the beginning section of the display.

The picture in the next column is the ending section of the display.

Please document CISP400V9A4.cpp, Date.cpp, Date.h, Time.cpp, and Time.h files properly and zip them into a proper named zip file for an assignment (refer to the assignment section of the class syllabus) and submit it to the A4 dropbox of the D2L Website.

Worth 150 points

AD4.

Modify the Time class of Figs. 9.4–9.5 (attached) to work with Date class, Date time class and employee class. The Time object should always remain in a consistent state.

Modify the Date and Employee class of Figs. 9.17- 9.20 (attached) to work with other class in the assignment.

Create DateTime class that includes a Time class object a composition, a tick member function that increments the time stored in a Date object by one second, and increaseADay function to increase day, month and year when it is proper.

In the CISP400V9AD4.cpp, we instantiate three Employee objects and assign them to the first three elements of a 10 element Employee pointer array. Use for loop to print out the each Employee object’s information before and after a set of training time.

The following is a description of each class.

Time class

The Time class has three private integer data members, hour (0 – 23 (24-hour clock format)), minute (0 – 59), and second (0 – 59).

It also has Time, setTime, setHour, setMinute, setSecond, getHour(), getMinute, getSecond,~Time, and printStandard public functions.

The Time function is a default constructor. It takes three integers and each has default value of 23, 59, and 58.The setTime function takes three integers but does not return any value. It initializes the private data members’ (hour, minute and second) data.The setHour function takes one integer but doesn’t return anything. It validates and stores the integer to the hour private data member.The setMinute function takes one integer but doesn’t return anything. It validates and stores the integer to the minute private data member.The setSecond function takes one integer but doesn’t return anything. It validates and stores the integer to the second private data member.The getHour constant function returns one integer but doesn’t take anything. It returns the private data member hour’s data.The getMinute constant function returns one integer but doesn’t take anything. It returns the private data member minute’s data.The getSecond constant function returns one integer but doesn’t take anything. It returns the private data member second’s data.The Time destructor does not take anything.The printStandard constant function does not return or accept anything. It displays time in standard-time format.

Date class

The Date class has three private integer data members (month, day and year), and one static constant integer variable (monthsPerYear).

It has Date, print, ~Date, setMonth, setYear, and setDay public functions. It has one private checkDay function.

1. The Date function is a default constructor. It takes 3 integers. The three integers have default data (1, 1, 1900).

2. The print constant function does not take or return data. It prints out the month, day and year information.

3. The ~Date function is a destructor of the Date class. It also displays “Date object destructor is called “; message and calls Time object destructor.

4. The setDay function takes an integer and does not return anything. It validates the day information by calling checkDay function and saves the validated information.

5. The setMonth function takes an integer and does not return anything. It validates the month information and saves the validated information.

6. The setYear function takes an integer and does not return anything. It validates the year information and saves the validated information. If year greater than 2020 or less than 1920 displays “invalid year and set to 2011’ information i

7. The constant checkDay function takes and returns an integer. It makes sure the accuracy of day, month, and year information. This utility function to confirm proper day value based on month and year, it also handles leap years, too.

DateTime class

The DateTime class has three private integer data members (month, day and year), one Time class object (time) and one static constant integer variable (monthsPerYear).

It has DateTime, print, increaseADay, tick, getMonth, getYear, getDay, setMonth, setYear, setDay, getHour, getMinute, getSecond, setHour, setMinute, setSecond, and ~DateTime public functions. It has one private checkDay function.

1. The DateTime function is a default constructor. It takes 3 integers and a Time object information. The three integers have default data of 0, 0, and 0. The Time object also has 0, 0, and 0 as default data.

2. The print constant function does not take or return data. It prints out the month, day, year and Time object information.

3. The increaseADay function does not take or return data. It increases the private data member day by one. It also checks the day to make sure the data is accurate. If the data is not accurate it will adjust all the necessary corresponding data.

4. The tick function does not takes or return data. It increases one second to the Time object of the DateTime class private data member. This function has to make sure that the second increased is proper or it will adjust all the necessary corresponding data.

5. The getMonth function returns an integer but does not take anything. It returns the month private data member.

6. The getYear function returns an integer but does not take anything. It returns the year private data member.

7. The getDay function returns an integer but does not take anything. It returns the day private data member.

8. The setDay function takes an integer and does not return anything. It validates the day information by calling checkDay function and saves the validated information.

9. The setMonth function takes an integer and does not return anything. It validates the month information and saves the validated information.

10. The setYear function takes an integer and does not return anything. It validates the year information and saves the validated information. If year greater than 2020 or less than 1920 displays “invalid year and set to 2011’ information i

11. The getHour function returns an integer but does not take anything. It returns the hour information of the Time object (time) private data member.

12. The getMinute function returns an integer but does not take anything. It returns the minute information of the Time object (time) private data member.

13. The getSecond function returns an integer but does not take anything. It returns the second information of the Time object (time) private data member.

14. The setHour function takes an integer but does not return anything. It validates the integer and set the validated information to hour component of the Time object (time) private data member.

15. The setMinute function takes an integer but does not return anything. It validates the integer and set the validated information to minute component of the Time object (time) private data member.

16. The setSecond function takes an integer but does not return anything. It validates the integer and set the validated information to the second component of theTime object (time) private data member.

17. The ~DateTime function is a destructor of the DateTime class.

18. The constant checkDay function takes and returns an integer. It makes sure the accuracy of day, month, and year information. This utility function to confirm proper day value based on month and year, it also handles leap years, too.

The Employee class has two private string data members (firstName and lastName), two private Date objects (hireDate and birthDate), two private DateTime objects (startDateTime and endDateTime), and one private static integer (count). The count is used to count the existence of Employee object.

It has Employee, getFirstName, getLastName, gethireDate, getbirthDate, getstartDateTime, getendDateTime, testZeroDateTime, setendDateTime, print, ~Employee, and getCount public functions.

The Employee function is a default constructor. It takes 2 strings, two Date objects, and two DateTime objects information.The getFirstName function returns a string but does not take any data. It returns the private data member firstName information.The getLastName function returns a string but does not take any data. It returns the private data member lastName information.The gethireDate function does not take or returns any data. It displays the private data member Date object hireDate information.The getbirthDate function does not take or returns any data. It displays the private data member Date object birthDate information.The getstartDateTime function does not take or returns any data. It displays the private data member DateTime object startDateTime information.The getendDateTime function does not take or returns any data. It displays the private data member DateTime object endDateTime information.The testZeroDateTime function takes a DateTime object and returns a Boolean data. It testes the passed in DataTime object whether the object contains all 0s in its data members. If yes than return true otherwise return false.The setendDateTime function takes three integers (hour, minute and second) but does not return anything. It takes the integers of training time needed for each employee to update the endDateTime object’s data members.The print function does not take or return any data. It displays an Empolyee object’s information. It shows employee’s first name last name, birth date, hire date, Training starts at, and Training ends at. If there is not training time set yet then displays “No specified end training date and time.”The ~Employee is the destructor of the class.The getCount static function does not take any data but return an integer. It returns the number of existence of the Employee class objects.

This assignment comes with a CISP400V9AD4.zip file. It includes eight files (CISP400V9AD4.cpp, CISP400V9AD4.exe, Date.cpp, Date.h, Time.cpp, Time.h, Employee.cpp, and Employee.h). The CISP400V9AD4.exe file is an executable file. You can double click the file to get to the expecting result (see the picture below) of this assignment. The Date.cpp, Date.h, Time.cpp, Time.h, Employee.cpp, and Employee.h are files coming from the textbook examples which you can use so you don’t need to start from scratch. After you finish your implementation for the Date, Time, DateTime, Employee classes, you can put the CISP400V9AD4.cpp, Date.cpp, Date.h, Time.cpp, Time.h, DateTime.cpp, DateTime.h, Employee.cpp, and Employee.h in a project and then you can run to the same result as the CISP400V9AD4.exe. Please be awarded that you can adjust only your program (Date.cpp, Date.h, Time.cpp, Time.h, DateTime.cpp, DateTime.h, Employee.cpp, and Employee.h) to generate the required result but not the code in CISP400V9AD4.cpp file.

The following is the display of the expecting result.

Please document CISP400V9AD4.cpp, Date.cpp, Date.h, Time.cpp, Time.h, DateTime.cpp, DateTime.h, Employee.cpp, and Employee.h files properly and zip them into a proper named zip file for an advance assignment (refer to the assignment section of the class syllabus) and submit it to the A4 dropbox of the D2L Website.

Worth 180 points