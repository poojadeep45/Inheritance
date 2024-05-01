package Pack1;  

// Superclass
public class Shape {
    
    // Method to get the area of a shape. 
    public double getArea(double area) {
        return area;
    }
    
    // Method to get the perimeter of a shape. 
    public double getPerimeter(double perimeter) {
        return perimeter;
    }
}

// Class representing a rectangle, inheriting from Shape
class Rectangle extends Shape {
    private double length;  // Length of the rectangle
    private double width;   // Width of the rectangle
    
    // Default constructor
    Rectangle() {
    }
    
    // Parameterized constructor to initialize length and width
    Rectangle(double length, double width) {
        this.length = length;
        this.width = width;
    }
    
    // Override the getArea method to calculate the area of a rectangle
    @Override
    public double getArea() {
        double area = length * width;  // Area formula for rectangle
        return area;
    }
    
    // Override the getPerimeter method to calculate the perimeter of a rectangle
    @Override
    public double getPerimeter() {
        double perimeter = 2 * (length + width);  // Perimeter formula for rectangle
        return perimeter;
    }
}

// Class representing a circle, inheriting from Shape
class Circle extends Shape {
    private double radius;  // Radius of the circle
    
    // Default constructor
    Circle() {
    }
    
    // Parameterized constructor to initialize radius
    Circle(double radius) {
        this.radius = radius;
    }
    
    // Override the getArea method to calculate the area of a circle
    @Override
    public double getArea() {
        double area = Math.PI * radius * radius;  // Area formula for circle
        return area;
    }
    
    // Override the getPerimeter method to calculate the perimeter of a circle
    @Override
    public double getPerimeter() {
        double perimeter = 2 * Math.PI * radius;  // Perimeter formula for circle
        return perimeter;
    }
}
