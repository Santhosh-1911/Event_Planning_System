Introduction

The Event Planning System is a database-driven project designed to manage events, participants, schedules, and payments efficiently. This SQL-based system helps in organizing events, tracking participant registrations, processing payments, and generating insights through stored procedures and views.
Database Schema
Tables:

    Events – Stores event details like event name, date, and location.

    Participants – Manages participant details including names and emails.

    EventSchedules – Keeps track of participant registrations for events.

    Payment – Records participant payments along with the mode of transfer.

Relationships:

    Each event can have multiple participants.

    Each participant can register for multiple events.

    Each participant can make a payment.

SQL Queries Included
1. Table Creation

    Defines the structure of the Events, Participants, EventSchedules, and Payment tables.

    Uses FOREIGN KEY constraints to establish relationships between tables.

2. Data Insertion

    Inserts sample data into all tables, including events, participants, schedules, and payments.

3. Stored Procedures

    GetAllEvents() – Retrieves all event details.

    GetOnlinePayments() – Fetches details of participants who made online payments.

    GetParticipantCountPerEvent() – Counts participants for each event.

    GetParticipantsForEvent(event_name_param) – Lists participants of a specific event.

    GetPaymentDetailsForParticipants() – Provides payment details of all participants.

    GetTotalCashPayments() – Returns the count of cash payments.

    GetParticipantsPaidAfterMarch1() – Retrieves participants who paid after March 1, 2025.

   4. Views

    MostPopularPaymentMode – Shows the most commonly used payment method.

    MostPopularEvent – Identifies the event with the highest number of participants.

    AvgParticipantsPerEvent – Calculates the average number of participants per event.



    MostPopularPaymentMode – Shows the most commonly used payment method.

    MostPopularEvent – Identifies the event with the highest number of participants.

    AvgParticipantsPerEvent – Calculates the average number of participants per event.
