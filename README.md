#  Comic-Con Event Parking System – ER Diagram

##  Overview

This project presents the database design for a **multi-zone parking management system** used during large-scale events like Comic-Con.
The system handles vehicle entry, parking allocation, session tracking, and payment processing across multiple zones and levels.

---

##  Problem Context

During the event, thousands of vehicles (bikes, cars, SUVs, EVs, etc.) arrive and need structured parking.
The system must support:

* Multiple parking zones and levels
* Reserved parking (VIP, staff, exhibitors, EV charging)
* Entry and exit tracking
* Parking spot allocation
* Ticket generation
* Payment handling

---

##  Key Entities

The ER diagram includes the following core entities:

* **Vehicle & VehicleCategory** – Stores vehicle details and types
* **ParkingZone, ParkingLevel, ParkingSpot** – Models parking hierarchy
* **ParkingSpotCategory** – Handles reserved and special spots
* **ParkingSession** – Tracks entry, exit, and spot usage
* **ParkingTicket** – Represents issued tickets
* **Payment** – Stores transaction details
* **AccessCategory & VehicleAccess** – Supports VIP, staff, and special roles
* **SpotAvailability** – Tracks real-time parking status

---

## Key Relationships

* One vehicle can have multiple parking sessions
* One parking spot can be reused across multiple sessions
* Parking spots belong to levels, and levels belong to zones
* Each session is linked to one ticket and one payment
* Vehicles can have multiple access categories (VIP, staff, etc.)

---

##  Features Supported

* Multi-entry support for vehicles across event days
* Real-time parking availability tracking
* Reserved parking management
* Accurate entry/exit timestamp tracking
* Payment calculation per session
* Identification of currently parked vehicles

---

## Image

<img width="1952" height="1152" alt="Comic-Con Parking System ER" src="https://github.com/user-attachments/assets/c3842c8d-ee73-4ac2-a0da-f486d87030fb" />


