/* Develop a program that allows a teacher to enter
students' grades and compute their average,
highest, and lowest scores. You can use arrays or
ArrayLists to store the student data. */



import java.util.ArrayList;
import java.util.Scanner;

public class StudentGrade{
 public static void main(String[] args) {
Scanner A = new Scanner(System.in);
ArrayList<Double> grades = new ArrayList<>();
String input;
System.out.println("Enter student grades (type 'done' to finish):");
while (true) {
System.out.print("Enter grade: ");
input = A.nextLine();
if (input.equalsIgnoreCase("done")) {
break; 
}
try {
double grade = Double.parseDouble(input); 
if (grade < 0 || grade > 100) {
System.out.println("Please enter a grade between 0 and 100.");
} else {
grades.add(grade); 
}
} catch (NumberFormatException e) {
System.out.println("Invalid input. Please enter a numeric grade."); 
}
}
if (grades.size() > 0) {
double sum = 0;
double highest = grades.get(0);
double lowest = grades.get(0);
for (double grade : grades) {
sum += grade; 
if (grade > highest) {
highest = grade; 
}
if (grade < lowest) {
lowest = grade; 
}
}
double average = sum / grades.size(); 
System.out.printf("Average grade: %.2f%n", average);
System.out.printf("Highest grade: %.2f%n", highest);
System.out.printf("Lowest grade: %.2f%n", lowest);
} else {
System.out.println("No grades were entered.");
}
A.close(); 
}
}
