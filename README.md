<h1>Jet2holidays Database Project</h1>

<h2>Overview</h2>
<p>This project involved reverse engineering the Jet2holidays.com website to design and implement a MySQL database representing its working structure. Jet2Holidays offers customers package holidays, including accommodation, travel arrangements, and additional services like insurance.

Our team focused on the main aspect of booking a direct flight and accommodation, with assumptions made regarding flight and accommodation availability. Features such as insurance or in-flight meals were deemed out of scope for this project.</p>

<h2>Entity Relationship Diagrams</h2>

We started by identifying the entity relationships from the Jet2Holidays website and created an entity relationship diagram to visualize the findings.

<h3><b>Figure 1. Here you can see the findings from the Entity Discovery exercise</b></h3>

![Entity Discovery](https://i.imgur.com/5zgbHhC.png)

<h3><b>Figure 2. Here you can see the Draw.io diagram showing the Entity Relationship</b></h3>

![Entity Relationship - Draw.io](https://i.imgur.com/p9iwkMV.png)

<h3><b>Figure 3. Here you can see the MySQL Designer diagram showing the Entity Relationship</b></h3>

![Entity Relationship - MySQL](https://i.imgur.com/7a7tdb8.png)

<h2>Development and Design Choices</h2>

The database evolved through continuous refinement and examination, with various tables added and removed to model the real-world relationships as closely as possible.

<h2>Design Features:</h2>

- Entity relation notation implementation
- Redundancy elimination
- Data integrity with foreign key constraints

<h2>Normalization:</h2>

- First Normal Form (1NF)
- Second Normal Form (2NF)
- Third Normal Form (3NF)

<h2>Examples of Good Design Choices</h2>

- Title Table: Created a separate table for titles to reduce redundancy.
- Airport Table: Introduced an airport_id attribute to maintain atomic data and reduce redundancy.
- Hotel Table & hotel_id: Implemented a hotel_id primary key linked to multiple related tables, allowing for atomic data and reduced redundancy.

<h2>Key Design Features</h2>

- Ability to book multiple flights and rooms under one booking
- Total price calculation for bookings
- Outsourced payment processing for security
- Different routes representation for flights
- Address geo-location for accurate location data
- Various data types used depending on the goal of the data held
- Soft delete feature excluded to avoid potential issues with data integrity and redundancy
