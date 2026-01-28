#simple python project
print("Welcome to Student Marks Calculator\n")
student_name = input("Enter student name: ")
number_of_subjects = int(input("Enter number of subjects: "))
total_marks = 0
for subject_number in range(1, number_of_subjects + 1):
    marks = int(input(f"Enter marks for subject {subject_number}: "))
    total_marks = total_marks + marks
percentage = total_marks / number_of_subjects
if percentage >= 90:
    grade = "A"
elif percentage >= 75:
    grade = "B"
elif percentage >= 50:
    grade = "C"
else:
    grade = "Fail"
print("\n----- Student Result -----")
print("Name       :", student_name)
print("Total Marks:", total_marks)
print("Percentage :", percentage)
print("Grade      :", grade)
