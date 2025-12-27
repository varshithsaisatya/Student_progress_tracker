#display title
print("--------------------------------------------")
print("      STUDENT PROGRESS TRACKER SYSTEM      ")
print("--------------------------------------------")

#taking basic student details as input
STUDENT_NAME = input("Enter the student name         : ")
STUDENT_CLASS = input("Enter the Student class        : ")
STUDENT_ROLL_NO = input("Enter the Student Roll number  :")

#taking number of subjects as input
Subjects = int(input("Enter the number of Subjects   : "))
print("")

print("============================================")

#total marks is starting 0
total = 0

# store failed subjects numbers
failed_subject=[]

for sub in range(1, Subjects + 1):
    marks = float(input(f"Enter your marks for subject {sub}: "))

    # Validate mark entry
    if marks > 100 or marks < 0:
        print("\033[31mInvalid marks! Please enter between 0 and 100.\033[0m")
        marks = float(input(f"\033[33mRe-enter marks for subject {sub}:\033[0m "))

    # Check fail subject
    if marks <= 34:
        print(f"\t\033[31m FAILED IN SUBJECT {sub} \033[0m")
        failed_subject.append(sub)
    total += marks
print("--------------------------------------------")
# Calculate average
average = total / Subjects
print("")
print(f"Total marks: {total}")
print(f"Average marks: {average}")

# Grade calculation and remarks based on average
if 90 <= average <= 100:
    GRADE="A"
    REMARKS="EXCELLENT"
elif 75 <= average <= 89:
    GRADE="B"
    REMARKS="VERY GOOD"
elif 50 <= average <= 74:
    GRADE="C"
    REMARKS="GOOD"
elif 35 <= average <= 49:
    GRADE="D"
    REMARKS="NEED IMPROVEMENT"
elif average <= 34:
    GRADE="F"
    REMARKS="FAILED"
print(f"Grade: {GRADE} - {REMARKS}")
print("============================================")
if len(failed_subject) == 0:
    RESULT="PASS"
    print(" YOU PASSED ALL SUBJECTS")
    print(f" RESULT: {RESULT}")
else:
    RESULT="FAIL"
    print(f" Total Failed Subjects: {len(failed_subject)}")
    print(f" Failed in: {failed_subject}")

#display student progress report
print("============================================")
print("--------------------------------------------")
print("         STUDENT PROGRESS REPORT            ")
print("--------------------------------------------")
print(f"STUDENT NAME     : {STUDENT_NAME}")
print(f"STUDENT CLASS    : {STUDENT_CLASS}")
print(f"STUDENT ROLL NO  : {STUDENT_ROLL_NO}")
print(F"TOTAL MARKS      : {total}")
print(f"STUDENT AVERAGE  : {average}")
print(f"STUDENT GRADE    : {GRADE}")
print(f"STUDENT RESULT   : {RESULT}")
print(f"REMARKS          : {REMARKS}")

# menu system
print("--------------------------------------------")
print("               MENU SYSTEM                  ")
print("--------------------------------------------")
print(" What Do You Want Next ?")
print("---------------------------------------------")

Choice=input("Enter your choice :")
while Choice!="4":
    if Choice=="1":

        print(f"The Total Marks: {total}")
        print("---------------------------------------------")
        Choice=input("Enter your choice :")
    elif Choice=="2":
        print(f"The Student Average: {average}")
        print("---------------------------------------------")
        Choice=input("Enter your choice :")

    elif Choice=="3":
        print("          STUDENT PROGRESS REPORT            ")
        print("---------------------------------------------")
        print(f"STUDENT NAME    :{STUDENT_NAME}")
        print(f"STUDENT CLASS   :{STUDENT_CLASS}")
        print(f"STUDENT ROLL NO :{STUDENT_ROLL_NO}")
        print(f"STUDENT AVERAGE :{average}")
        print(f"STUDENT GRADE   :{GRADE}")
        print(f"STUDENT RESULT  :{RESULT}")
        print(f"REMARKS         :{REMARKS}")
        print("---------------------------------------------")
        Choice=input("Enter your choice :")
        print("---------------------------------------------")
    elif Choice=="4":
        exit
print(" THANK YOU_ ")
print("---------------------------------------------")
