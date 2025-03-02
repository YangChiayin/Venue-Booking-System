# Venue Booking System
<img src="https://github.com/user-attachments/assets/a20e284f-f542-4fc1-a62b-d27a2bc25fd7" width="500" />

This application allows users to book seats, add themselves to a waitlist, and cancel bookings for a venue with a limited number of seats. The application is developed using **C# with a Windows Forms interface**, providing an interactive way to manage bookings.

## Key Features

- **Book Seats:** Users can select a seat, enter their username, and book the seat. Booked seats are visually marked and are no longer available for others.
- **Waitlist Management:** If all seats are booked, users are added to the waitlist.
- **Cancel Bookings:** Users can cancel their bookings and free up seats for others. The seat will be given to the first person on the waitlist if any.
- **Fill All Seats:** Allows the user to book all vacant seats in one go.
- **Clear All Bookings:** The option to cancel all bookings, including clearing the waitlist.
- **Seat Availability Display:** The application continuously displays the current available seats and the booking capacity.

## Getting Started

### 1. **Prerequisites:**
   - Visual Studio or any other C# development environment

### 2. **Installation:**
   - Download the project source code.
   - Open the `*.sln` file in Visual Studio.

### 3. **Running the Application:**
   - Build the solution in Visual Studio.
   - Run the executable from Visual Studio or from the `bin\Debug` or `bin\Release` folder.

## Usage

### 1. **Booking a Seat:**
   - Select a row and column for the seat.
   - Enter a username and click "Book Seat".
   - If the seat is available, it will be booked and the seat button color will change to red.
   - If the seat is already booked, a message will appear stating that the seat is unavailable.

### 2. **Adding to Waitlist:**
   - If all seats are booked, users can click "Add to Waitlist".
   - The application will add them to the waitlist and notify them of their successful addition.

### 3. **Canceling a Booking:**
   - Users can cancel a seat booking by entering their username and selecting the row and column.
   - If the seat is booked by the user, it will be canceled. The seat will be assigned to the first person on the waitlist, if any.

### 4. **Cancel All Bookings:**
   - Click "Cancel All Bookings" to reset all bookings and the waitlist.
   - All seats will be freed and reset to their original state.

### 5. **Fill All Vacant Seats:**
   - Users can fill all vacant seats with their username by clicking "Fill All Seats".
   - This will automatically book all empty seats and display the updated seat status.

### 6. **Seat Availability:**
   - The current available seat count and booking capacity are shown in the `lblStatus` label. It updates dynamically as users make bookings or cancellations.

## Data Structure

- **Venue Layout:** The venue consists of 3 rows (A, B, C) and 4 columns (1, 2, 3, 4), for a total of 12 seats.
- **Waitlist:** If all seats are occupied, the system adds users to a waitlist.

## Seat Availability Example

When booking a seat or filling all vacant seats, the seat layout is updated. A booked seat will be marked red, and available seats are marked with a light green color.
