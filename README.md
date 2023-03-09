package assignment;

public class CalculateG {
	 public static double multiply(double a, double b) {
	        return a * b;
	    }

	    public static double square(double a) {
	        return Math.pow(a, 2);
	    }

	    public static double sum(double a, double b) {
	        return a + b;
	    }

	    public static void printResult(String message, double result) {
	        System.out.println(message + result);
	    }

	public static void main(String[] args) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double fallingTime = 30; 
        double initialVelocity = 0.0; 
        double finalVelocity;
        double initialPosition = 0.0; 
        double finalPosition;

        finalVelocity = sum(initialVelocity, multiply(gravity, fallingTime));
        finalPosition = 0.5 * multiply(gravity, square(fallingTime)) + multiply(initialVelocity, fallingTime) + initialPosition;

        printResult("The object's final velocity is ", finalVelocity);
        printResult("The object's final position is ", finalPosition);
        

	}

}
