public class ScientificCalculator {

    public double add(double a, double b) {
        return a + b;
    }

    public double subtract(double a, double b) {
        return a - b;
    }

    public double multiply(double a, double b) {
        return a * b;
    }

    public double divide(double a, double b) {
        if (b == 0) throw new ArithmeticException("Cannot divide by zero");
        return a / b;
    }

    public double power(double base, double exponent) {
        return Math.pow(base, exponent);
    }

    public double squareRoot(double num) {
        if (num < 0) throw new ArithmeticException("Cannot calculate square root of a negative number");
        return Math.sqrt(num);
    }

    public double sine(double angle) {
        return Math.sin(Math.toRadians(angle));
    }

    public double cosine(double angle) {
        return Math.cos(Math.toRadians(angle));
    }

    public double tangent(double angle) {
        if (angle % 180 == 90) throw new ArithmeticException("Tangent is undefined at 90 degrees and odd multiples.");
        return Math.tan(Math.toRadians(angle));
    }

    public static void main(String[] args) {
        ScientificCalculator calculator = new ScientificCalculator();
        Scanner scanner = new Scanner(System.in);
        boolean exit = false;

        System.out.println("Welcome to the Scientific Calculator!");

        while (!exit) {
            System.out.println("\nChoose an operation:");
            System.out.println("1. Addition (+)");
            System.out.println("2. Subtraction (-)");
            System.out.println("3. Multiplication (*)");
            System.out.println("4. Division (/)");
            System.out.println("5. Power (x^y)");
            System.out.println("6. Square Root (√x)");
            System.out.println("7. Sine (sin)");
            System.out.println("8. Cosine (cos)");
            System.out.println("9. Tangent (tan)");
            System.out.println("0. Exit");

            System.out.print("Enter choice (0-9): ");
            int choice = scanner.nextInt();

            switch (choice) {
                case 1 -> {
                    System.out.print("Enter first number: ");
                    double num1 = scanner.nextDouble();
                    System.out.print("Enter second number: ");
                    double num2 = scanner.nextDouble();
                    System.out.println("Result: " + calculator.add(num1, num2));
                }
                case 2 -> {
                    System.out.print("Enter first number: ");
                    double num1 = scanner.nextDouble();
                    System.out.print("Enter second number: ");
                    double num2 = scanner.nextDouble();
                    System.out.println("Result: " + calculator.subtract(num1, num2));
                }
                case 3 -> {
                    System.out.print("Enter first number: ");
                    double num1 = scanner.nextDouble();
                    System.out.print("Enter second number: ");
                    double num2 = scanner.nextDouble();
                    System.out.println("Result: " + calculator.multiply(num1, num2));
                }
                case 4 -> {
                    System.out.print("Enter first number: ");
                    double num1 = scanner.nextDouble();
                    System.out.print("Enter second number: ");
                    double num2 = scanner.nextDouble();
                    try {
                        System.out.println("Result: " + calculator.divide(num1, num2));
                    } catch (ArithmeticException e) {
                        System.out.println("Error: " + e.getMessage());
                    }
                }
                case 5 -> {
                    System.out.print("Enter base number: ");
                    double base = scanner.nextDouble();
                    System.out.print("Enter exponent: ");
                    double exponent = scanner.nextDouble();
                    System.out.println("Result: " + calculator.power(base, exponent));
                }
                case 6 -> {
                    System.out.print("Enter number: ");
                    double num = scanner.nextDouble();
                    try {
                        System.out.println("Result: " + calculator.squareRoot(num));
                    } catch (ArithmeticException e) {
                        System.out.println("Error: " + e.getMessage());
                    }
                }
                case 7 -> {
                    System.out.print("Enter angle in degrees: ");
                    double angle = scanner.nextDouble();
                    System.out.println("Result: " + calculator.sine(angle));
                }
                case 8 -> {
                    System.out.print("Enter angle in degrees: ");
                    double angle = scanner.nextDouble();
                    System.out.println("Result: " + calculator.cosine(angle));
                }
                case 9 -> {
                    System.out.print("Enter angle in degrees: ");
                    double angle = scanner.nextDouble();
                    try {
                        System.out.println("Result: " + calculator.tangent(angle));
                    } catch (ArithmeticException e) {
                        System.out.println("Error: " + e.getMessage());
                    }
                }
                case 0 -> {
                    exit = true;
                    System.out.println("Exiting the calculator. Goodbye!");
                }
                default -> System.out.println("Invalid choice. Please choose a valid operation.");
            }
        }

        scanner.close();
    }
}
