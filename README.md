import java.util.Scanner;

public class MovieBookingSystem {
  static int availableSeats = 20;

  public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);

    System.out.println("Welcome to the Movie Ticket Booking System");
    System.out.println("Available seats: " + availableSeats);

    while (true) {
      System.out.print("Enter the number of seats to book (or 0 to exit): ");
      int numSeats = sc.nextInt();
      if (numSeats == 0) {
        break;
      }
      if (numSeats > availableSeats) {
        System.out.println("Sorry, we only have " + availableSeats + " seats available.");
      } else {
        availableSeats -= numSeats;
        System.out.println("Booking confirmed! Enjoy the movie.");
        System.out.println("Available seats: " + availableSeats);
      }
    }
    System.out.println("Thanks for using the movie ticket booking system.");
  }
}
