# Airline-Reservation-System
This Entity-Relationship Diagram (ERD) represents an Airline Reservation System with the following entities and relationships :

TRAVELLER: Includes attributes like ID (primary key), First_name, Phone_no, Address, Gender, and Age. Travellers can check for flights, book tickets, or cancel reservations.
FLIGHT: Contains attributes such as Flight_no (primary key), Flight_name, Dep_time, Destination, Distance, Seat_available, Source, and Airlines. Flights belong to an AIRLINE and have a CLASS.
AIRLINE: Has attributes like Airline_name and Contact_no. An airline manages multiple FLIGHTS.
CLASS: Includes Economy and Business types, with attributes Fare, Class_type, and Flight_no. A FLIGHT can have multiple classes, represented as a generalization hierarchy.
TICKET: Contains attributes like Traveller_name, Flight_no, Date/time, Seat_no, and Class. A TRAVELLER books a TICKET, and a TICKET can be canceled. A TICKET is also received after payment.
PAYMENT: Includes attributes like Transaction_ID (primary key), Amount, and Payment_mode. A PAYMENT is made to confirm a TICKET booking.
# Relationships:

A TRAVELLER checks for a FLIGHT.
A TRAVELLER books or cancels a TICKET.
A FLIGHT belongs to an AIRLINE.
A FLIGHT has one or more CLASS types (Economy or Business).
A TICKET is received after a PAYMENT is made.
A TICKET is associated with one FLIGHT and one TRAVELLER.
 The ERD uses diamonds for relationships (e.g., "check for," "book," "cancel," "has," "belongs to," "receive") and ovals for attributes, with primary keys underlined. A triangle indicates the generalization of CLASS into Economy and Business.
