# Lab12-RelationalDatabases
## Tables
### Hotel Information
This table holds information about each specific Hotel including: Hotel Name, Hotel Location, Number of Rooms, and Phone Number. This table also has its own ID which is shared with two other tables: Room Lookup and Hotel Records.
### Room Information
This table holds information about specific Rooms including: Guest Name, Room Name, Room Layout, Price, Amenities, and Pet Friendly status. This table has its own ID which is shared with two other tables: Room Lookup and Hotel Records. Room Information also pulls from an enum which holds Room Layouts.
### Room Lookup
This table is only a Join table. It takes keys from the Hotel Informationt table and the Room Information table.
### Records
This table is a Joint Entity Table with a Payload. It takes data from the Hotel Information table and the Room Information table. It also adds information: Date of Guest Check In, Date of Guest Check Out, and Condition of Room at Checkout.
### Room Layout
This enum holds Room Layouts including: Studio, One Bedroom, and Two Bedroom.  It is used exclusively by the Room Information table.