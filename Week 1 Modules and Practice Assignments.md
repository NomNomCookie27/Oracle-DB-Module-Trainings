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
