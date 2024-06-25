import java.util.Scanner;

public class FacebookLoginSystem {
    private static final String CORRECT_USERNAME = "user123";
    private static final String CORRECT_PASSWORD = "pass123";

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to Facebook Login System");
        System.out.print("Enter your username: ");
        String username = scanner.nextLine();

        System.out.print("Enter your password: ");
        String password = scanner.nextLine();
        if (username.equals(CORRECT_USERNAME) && password.equals(CORRECT_PASSWORD)) {
            System.out.println("Login successful! Welcome " + username);
        } else {
            System.out.println("Invalid username or password. Please try again.");
        }
    }
}
