public class main {
    public static void main(String[] args) {
        // Create a Student object and initialize it with sample data
        Student student = new Student("syedkhaleel", 27, "A");

        // Display the student's information
        student.displayInfo();

        // Update the student's grade
        student.updateGrade("A");

        // Display the updated information
        System.out.println("\nUpdated Student Info:");
        student.displayInfo();
    }
}

public class Student {
    // Private instance variables
    private String name;
    private int age;
    private String grade;

    // Constructor
    public Student(String name, int age, String grade) {
        this.name = name;
        this.age = age;
        this.grade = grade;
    }

    // Method to display student's information
    public void displayInfo() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Grade: " + grade);
    }

    // Method to update the student's grade
    public void updateGrade(String newGrade) {
        this.grade = newGrade;
    }
}
