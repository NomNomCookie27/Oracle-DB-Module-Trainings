## Section 1.1: Introduction to Databases

### What I Learned:
- Databases are systems for organizing, storing, and managing data.
- Different types like Hierarchical, Network, and Relational databases handle various data structures.

### Key Takeaways:
- Databases help keep data organized for easy access and updates.
- Each database type has strengths suited to different data scenarios.

### Practice Assignment: Identify Key Concepts

- **Purpose of a Database**:
  - Databases keep information organized, making it easy to find and manage, supporting everyday operations like business and school systems.

- **Types of Databases**:
  - **Hierarchical Database**: Data is in a tree-like structure with parent-child relationships. Example: A company’s organizational chart.
  - **Network Database**: Supports complex many-to-many relationships. Example: Airline routes connecting multiple cities.
  - **Relational Database**: Data is stored in tables linked by keys. Example: Customer management where customers and orders are connected by IDs.

## Section 1.2: Data Modeling

### What I Learned:
- Data modeling involves designing how data is stored and related in a database.
- Good models help store data correctly and efficiently.

### Key Takeaways:
- Models show entities, attributes, and relationships before building the database.
- Modeling is crucial for a well-structured database.

### Practice Assignment 1: Create a Student Registration System

- **Entities and Attributes**:

  | Entity     | Attributes              | Description                                  |
  |------------|-------------------------|----------------------------------------------|
  | Student    | Student ID, Name, DOB   | Details of each student, like a unique ID.   |
  | Course     | Course ID, Course Name  | Information about courses offered.           |
  | Enrollment | Enrollment Date, Status | Links students to courses they take.         |
  | Teacher    | Teacher ID, Name        | Details about teachers and their departments.|

- **Relationships**:
  - Students enroll in many courses, and each course can have many students. This is managed through the Enrollment table.
  - Teachers can teach multiple courses, and each course is taught by one teacher.

### Practice Assignment 2: Library Management System

- **Entities and Attributes**:

  | Entity  | Attributes               | Description                                |
  |---------|--------------------------|--------------------------------------------|
  | Books   | Book ID, Title, Author   | Information about books in the library.    |
  | Members | Member ID, Name, Contact | Details of library members.                |
  | Loans   | Loan ID, Loan Date       | Tracks which books members borrow.         |
  | Staff   | Staff ID, Role           | Information about library staff.           |

- **Connections**:
  - Members borrow books, tracked by Loans connecting members to books.
  - Staff help manage loans and assist members.

## Section 1.3: Types of Database Models

### What I Learned:
- Different database models structure data differently, each with its advantages.
- Understanding each model helps choose the right one for specific needs.

### Key Takeaways:
- Models include Flat File, Hierarchical, Network, Relational, and Object-Oriented.
- Each model is best for different types of data and relationships.

### Practice Assignment: Identify the Database Models

- **Flat File Model**: Single table without structured relationships. Example: A simple spreadsheet with customer and order details together.
- **Hierarchical Model**: Tree structure with one-to-many relationships. Example: Organizational charts.
- **Network Model**: Web-like, many-to-many relationships. Example: A social network.
- **Relational Model**: Tables with defined relationships using keys. Example: A school database with students, courses, and enrollments.
- **Object-Oriented Model**: Combines database functions with programming objects. Example: User profiles stored as objects in a software system.

## Section 1.4: Business Requirements

### What I Learned:
- Business requirements shape database design, guiding how data is structured.
- Business rules affect the organization and management of data.

### Key Takeaways:
- Business needs are translated into database designs that support organizational goals.
- Business rules guide how data is linked and stored.

### Practice Assignment: Analyze Business Scenarios

- **LibBook Digital Library**:
  - Different membership types: Corporate, Student, and Individual.
  - Only students have free memberships; others pay fees.
  - Membership changes are allowed with valid reasons.

- **Star Care Hospital**:
  - Doctors need at least seven years of experience.
  - Patients and doctors are identified by unique IDs.

  ## Section 2.1: Relational Databases

### What I Learned:
- Relational databases use tables, keys, and relationships to organize data.
- Tables link through primary and foreign keys, making complex queries possible.

### Key Takeaways:
- Designing tables with the right keys and relationships helps manage data effectively.
- Relational databases are flexible for various business needs.

### Practice Assignment: Analyze Features of Relational Databases

- **Book.com Online Store**:
  - Tables include Books, Authors, Customers, and Shopping Carts. Each table has specific fields and connections, like ISBN linking Books with Orders.

  | Table        | Key Fields             | Description                                |
  |--------------|------------------------|--------------------------------------------|
  | Books        | ISBN, Title, AuthorID  | Details of books, linked by ISBN.          |
  | Authors      | AuthorID, Name         | Information on book authors.               |
  | Customers    | CustomerID, Name       | Customer details with order history.       |
  | Shopping Carts | CartID, CustomerID   | Tracks items in customers’ shopping carts. |

- **ABC Ltd Sales and Stock Control**:
  - Tables manage orders, products, invoices, and payments.

  | Table     | Key Fields            | Description                               |
  |-----------|-----------------------|-------------------------------------------|
  | Orders    | OrderID, CustomerID   | Tracks customer orders and statuses.      |
  | Products  | ProductID, Name       | Information about products in stock.      |
  | Invoices  | InvoiceID, OrderID    | Billing details linked to orders.         |
  | Payments  | PaymentID, InvoiceID  | Records payments made by customers.       |

## Section 2.2: Conceptual and Physical Data Models

### What I Learned:
- Conceptual models show how data is organized without technical details.
- Physical models detail the actual structure of the database.

### Key Takeaways:
- Conceptual models are used for planning; physical models guide database creation.
- Translating concepts to physical designs involves specifying tables, keys, and data types.

### Practice Assignment: Compare Conceptual and Physical Models

- **Conceptual Model**:
  - High-level design showing entities and relationships without focusing on specifics like data types.

- **Physical Model**:
  - Detailed representation with table structures, data types, keys, and indexes.

- **Example**: For a student system, I started with a conceptual model showing Students, Courses, and Enrollments, then built a physical model detailing the exact table structures and constraints.

## Section 2.3: Entities and Attributes

### What I Learned:
- Entities are main objects in a database; attributes describe these objects.
- Defining attributes helps organize data and ensures it’s stored correctly.

### Key Takeaways:
- Identifying key entities and their attributes helps build a clear database structure.
- Separating required and optional attributes is crucial for accurate data entry.

### Practice Assignment: Define Entities and Attributes for a School Management System

- **Entities and Attributes**:

  | Entity     | Attributes                       | Required? |
  |------------|----------------------------------|-----------|
  | Student    | Student ID, Name, Date of Birth | Yes       |
  | Course     | Course ID, Course Name           | Yes       |
  | Faculty    | Faculty ID, Name, Email          | Yes       |
  | Department | Department ID, Name              | No        |

- **Details**:
  - I listed each entity’s attributes, marking which are mandatory, like Student ID for students and Course ID for courses.

## Section 2.4: Unique Identifiers

### What I Learned:
- Primary keys uniquely identify records; foreign keys connect related tables.
- Keys are essential for maintaining data integrity and linking data.

### Key Takeaways:
- Identifying correct primary and foreign keys is key to building functional tables.
- Unique identifiers prevent duplication and maintain data consistency.

### Practice Assignment: Identify Unique Identifiers and Add to ERD

- **Primary and Foreign Keys**:

  | Entity   | Primary Key  | Alternative Key         | Description                      |
  |----------|--------------|-------------------------|----------------------------------|
  | Student  | Student ID   | Email Address           | Unique ID for each student.      |
  | Locker   | Locker Number| Location + Owner Name   | Each locker identified by number.|

- **Details**:
  - I assigned keys to relevant fields, such as Student ID as the primary key, linking tables correctly in the ERD.
## Section 2.5: Relationships

### What I Learned:
- Relationships define data flow between entities, showing how they interact.
- Modeling these relationships helps in understanding the overall structure.

### Key Takeaways:
- Defining one-to-many and many-to-many relationships clarifies data connections.
- ERDs help visualize these links, making complex interactions easier to manage.

### Practice Assignment: Analyze and Model Relationships

- **Relationships Modeled**:
  - Students enroll in many courses, managed through an Enrollment table linking the Student and Course entities.
  - Teachers teach multiple courses, connected through a one-to-many relationship.

- **ERD Representation**:
  - I drew diagrams showing clear links between students and courses through the Enrollment table, demonstrating data flow.

## Section 2.6: Entity Relationship Modeling (ERDs)

### What I Learned:
- ERDs represent the structure of a database, showing entities, attributes, and relationships.
- Drawing ERDs helps visualize how data is organized and linked.

### Key Takeaways:
- Creating ERDs helps in planning and communicating the database design.
- ERDs are useful for both technical teams and stakeholders to understand data flow.

### Practice Assignment: Identify Components and Draw ERDs

- **Components Identified**:
  - Main entities like Student, Course, and Enrollment, with their attributes and connections.

- **ERD Details**:
  - I included primary and foreign keys in the ERD to illustrate how data is linked across the system.

## Section 3.1: More with Relationships

### What I Learned:
- Many-to-many relationships can be managed using intermediate tables that link entities.
- Resolving these relationships helps maintain a clear database structure.

### Key Takeaways:
- Linking tables simplify complex many-to-many connections.
- Constraints and keys organize data, reducing redundancy.

### Practice Assignment: Resolve M:M Relationships and Add Constraints

- **Entities and Attributes**:

  | Entity       | Attributes              | Description                              |
  |--------------|-------------------------|------------------------------------------|
  | Student      | Student ID, Name        | Basic details of the student.            |
  | Course       | Course ID, Course Name  | Information about each course offered.   |
  | Enrollment   | Enrollment ID, Date     | Links students and courses.              |

- **Relationship Resolution**:
  - The Enrollment table connects students and courses, resolving many-to-many relationships.

- **Example**:
  - I showed how student IDs and course IDs are linked in the Enrollment table, adding constraints to prevent duplicate enrollments.

## Section 3.2: Tracking Data Changes

### What I Learned:
- Tracking changes over time helps keep an accurate record of data updates.
- Designing ERDs to include timestamps or history tables maintains both current and past records.

### Key Takeaways:
- Tracking historical data is important for analysis and accountability.
- Modifying ERDs to include time-based attributes helps manage changes.

### Practice Assignment: Construct ERDs for Time-Related Scenarios

- **ERD Modifications**:
  - Added attributes like `CreatedDate` and `ModifiedDate` to track when data is added or changed.

- **Example**:
  - In the Student Registration System, I added a `GradeHistory` table to keep records of grades over time, showing changes semester by semester.

## Section 3.3: Normalization and Business Rules

### What I Learned:
- Normalization organizes data to reduce redundancy and improve consistency.
- Business rules guide how data should be structured to meet specific needs.

### Key Takeaways:
- Normalization steps (1NF, 2NF, 3NF) streamline data structure.
- Following business rules during design helps align the database with organizational goals.

### Practice Assignment: Normalize Data and Apply Business Rules

- **Normalization Steps**:

  | Step       | Action                              | Resulting Table             |
  |------------|-------------------------------------|-----------------------------|
  | Unnormalized| Data with repeated values          | Single flat table           |
  | 1NF        | Split multi-valued attributes       | Separate tables             |
  | 2NF        | Remove partial dependencies         | Linked tables efficiently   |
  | 3NF        | Remove transitive dependencies      | Fully normalized structure  |

- **Details**:
  - I transformed a sample dataset into normalized tables, starting with unnormalized data and gradually organizing it to meet 3NF requirements.

- **Example**:
  - Final tables included Customers, Orders, and Products, each connected without duplication, following business rules to maintain data integrity.

## Section 3.4: Data Modeling Terminology and Mapping

### What I Learned:
- Data modeling terms help translate designs into physical tables in a database.
- Mapping ensures that entities, attributes, and relationships are accurately represented.

### Key Takeaways:
- Mapping ERD components to physical designs keeps the database aligned with its initial model.
- Using consistent naming and rules helps maintain a clear and usable structure.

### Practice Assignment: Identify and Map ERD Elements

- **Mapping Components**:
  - Analyzed an ERD and mapped entities to physical tables, assigning column names and defining keys.

- **Example**:
  - I mapped a Product entity from the ERD to a physical table with columns like `ProductID`, `Name`, and `Price`, ensuring the design matched real-world requirements.
