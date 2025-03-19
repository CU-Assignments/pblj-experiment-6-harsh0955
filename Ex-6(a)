import java.util.ArrayList;
import java.util.Collections;
import java.util.Comparator;
import java.util.List;

class Employee {
    private String name;
    private int age;
    private double salary;

    public Employee(String name, int age, double salary) {
        this.name = name;
        this.age = age;
        this.salary = salary;
    }

    public String getName() {
        return name;
    }

    public int getAge() {
        return age;
    }

    public double getSalary() {
        return salary;
    }

    @Override
    public String toString() {
        return "Employee{" +
                "name='" + name + '\'' +
                ", age=" + age +
                ", salary=" + salary +
                '}';
    }
}

public class EmployeeSorter {
    public static void main(String[] args) {
        List<Employee> employees = new ArrayList<>();
        employees.add(new Employee("Alice", 30, 70000));
        employees.add(new Employee("Bob", 25, 50000));
        employees.add(new Employee("Charlie", 35, 80000));
        employees.add(new Employee("David", 28, 60000));

        // Sort by name
        Collections.sort(employees, Comparator.comparing(Employee::getName));
        System.out.println("Sorted by name:");
        employees.forEach(System.out::println);

        // Sort by age
        Collections.sort(employees, Comparator.comparingInt(Employee::getAge));
        System.out.println("\nSorted by age:");
        employees.forEach(System.out::println);

        // Sort by salary
        Collections.sort(employees, Comparator.comparingDouble(Employee::getSalary));
        System.out.println("\nSorted by salary:");
        employees.forEach(System.out::println);
    }
}
