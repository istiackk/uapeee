# uapeee

This code is a simple movie ticket management system implemented in the C programming language. It allows users to book movie tickets by providing their name, email, phone number, and a default password. The system then provides options to view the movie schedule and book tickets for specific shows.

Here's a breakdown of the code:

1. It includes the standard input-output library `stdio.h`.

2. In the `main` function:
   - It declares several variables to store user information, password, and other data.
   - It opens a file named "ticket.txt" in append mode. If the file doesn't exist, it prints a message indicating that the file could not be created.
   - If the file is successfully opened, the program proceeds to collect user information.

3. The user is prompted to enter their name, email, phone number, and a default password (which is set to 123).

4. The code checks the entered password, and if it's correct (123), it provides a menu of options:
   - Press 1 to view the movie schedule.
   - Press 2 to book tickets.
   - Any other key to exit.

5. If the user selects the option to view the movie schedule (Press 1), it displays a list of available movies and their showtimes.

6. If the user selects the option to book tickets (Press 2), the code asks for a movie code. If the code is valid (between 1 and 5), it proceeds to choose a seat number from 1 to 6 and displays the user's information along with the booked seat and the ticket cost (set to 350 Taka). It also updates the available and booked seat count.

7. If the user enters an invalid movie code, it prints an error message.

8. If the user enters an invalid option, it displays a "Sorry, you have entered the wrong keyword" message.

9. The code then closes the file and returns 0 to indicate successful execution.

This code is a basic movie ticket booking system, but it lacks some important features like error handling, data validation, and proper user authentication. Additionally, it doesn't contain any loops, so after booking one ticket, the program will exit.
