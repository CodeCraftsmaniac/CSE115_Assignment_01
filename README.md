CSE115 Assignment 01

#include <stdio.h>
#include <math.h>

int main() {
    //Homework Question 1 - Lab Manual 2

    double x, result1;
    printf("Enter the value of x: ");
    scanf("%lf", &x);
    result1 = 5*x*x*x - 4*x*x + sqrt(x) + 3;
    printf("Result of problem 1: %.2f\n", result1);


   // Homework Question 2 - Lab Manual 2

    double a, b, c, discriminant, root1, root2;
    printf("Enter the values of a, b, c: ");
    scanf("%lf %lf %lf", &a, &b, &c);
    discriminant = b*b - 4*a*c;
    root1 = (-b + sqrt(discriminant)) / (2*a);
    root2 = (-b - sqrt(discriminant)) / (2*a);
    printf("Root 1: %.2f\nRoot 2: %.2f\n", root1, root2);


   // Homework Question 3 - Lab Manual 2

    double side, height, diameter, cubeVolume, cylinderVolume;
    printf("Enter the side length of the cube: ");
    scanf("%lf", &side);
    cubeVolume = side * side * side;
    printf("Volume of cube: %.2f\n", cubeVolume);

    printf("Enter the height and diameter of the cylinder: ");
    scanf("%lf %lf", &height, &diameter);
    cylinderVolume = M_PI * (diameter/2) * (diameter/2) * height;
    printf("Volume of cylinder: %.2f\n", cylinderVolume);



 // Homework Question 4 - Lab Manual 2


    int num1, num2, quotient1, remainder1, quotient2, remainder2;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    quotient1 = num1 / num2;
    remainder1 = num1 % num2;
    quotient2 = num2 / num1;
    remainder2 = num2 % num1;
    printf("Quotient and remainder of %d divided by %d: %d, %d\n", num1, num2, quotient1, remainder1);
    printf("Quotient and remainder of %d divided by %d: %d, %d\n", num2, num1, quotient2, remainder2);


    // Homework Question 5 - Lab Manual 2

    double celsius, fahrenheit;
    printf("Enter temperature in Celsius: ");
    scanf("%lf", &celsius);
    fahrenheit = (celsius * 9/5) + 32;
    printf("Temperature in Fahrenheit: %.2f\n", fahrenheit);



 // Homework Question 1 - Lab Manual 3


    double base1, base2, heightTrap, heightParallelogram, areaTrapezoid, areaParallelogram;
    printf("Enter the bases and height of the trapezoid: ");
    scanf("%lf %lf %lf", &base1, &base2, &heightTrap);
    areaTrapezoid = 0.5 * (base1 + base2) * heightTrap;
    printf("Area of trapezoid: %.2f\n", areaTrapezoid);

    printf("Enter the base and height of the parallelogram: ");
    scanf("%lf %lf", &base1, &heightParallelogram);
    areaParallelogram = base1 * heightParallelogram;
    printf("Area of parallelogram: %.2f\n", areaParallelogram);

   // Homework Question 2 - Lab Manual 3


    double radius, heightCone, volumeCone, surfaceAreaCone;
    printf("Enter the radius and height of the cone: ");
    scanf("%lf %lf", &radius, &heightCone);
    volumeCone = M_PI * radius * radius * heightCone / 3;
    surfaceAreaCone = M_PI * radius * (radius + sqrt(radius*radius + heightCone*heightCone));
    printf("Volume of cone: %.2f\nSurface area of cone: %.2f\n", volumeCone, surfaceAreaCone);


  // Homework Question 3 - Lab Manual 3

    double base, triangleHeight, hypotenuse;
    printf("Enter the base and height of the right angle triangle: ");
    scanf("%lf %lf", &base, &triangleHeight);
    hypotenuse = sqrt(base*base + triangleHeight*triangleHeight);
    printf("Length of hypotenuse: %.2f\n", hypotenuse);

    return 0;
}
