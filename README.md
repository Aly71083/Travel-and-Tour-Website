# Happy Feets Tour Booking System

A web-based tour booking system built with Java EE (Jakarta EE) and MySQL.

## Features

- User Registration and Login
- Tour Package Browsing
- Tour Booking Management
- User Profile Management
- Admin Dashboard
- Secure Payment Processing

## Technology Stack

- **Backend**: Java EE (Jakarta EE 9)
- **Frontend**: JSP, JSTL, HTML5, CSS3, JavaScript
- **Database**: MySQL 8.0
- **Server**: Apache Tomcat 10.0
- **Build Tool**: Maven

## Prerequisites

- Java JDK 11 or higher
- MySQL 8.0 or higher
- Apache Tomcat 10.0 or higher
- Eclipse IDE for Enterprise Java Developers
- Maven 3.6 or higher

## Project Structure

```
tourcode/
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── happyfeets/
│                   ├── controller/
│                   ├── dao/
│                   ├── model/
│                   └── util/
├── WebContent/
│   ├── WEB-INF/
│   │   ├── lib/
│   │   ├── db/
│   │   └── web.xml
│   ├── META-INF/
│   │   └── context.xml
│   ├── admin/
│   ├── includes/
│   └── *.jsp
└── pom.xml
```

## Database Setup

1. Open MySQL Workbench
2. Create a new connection to your MySQL server
3. Execute the `schema.sql` file located in `WebContent/WEB-INF/db/`
4. The script will:
   - Create the `happyfeets` database
   - Create all necessary tables
   - Insert sample data

## Configuration

1. **Database Configuration**:
   - Update `WebContent/META-INF/context.xml` with your MySQL credentials:
   ```xml
   <Resource name="jdbc/happyfeets" 
             auth="Container"
             type="javax.sql.DataSource"
             username="your_username"
             password="your_password"
             ... />
   ```

2. **Server Configuration**:
   - Configure Tomcat server in Eclipse
   - Set up deployment assembly
   - Configure targeted runtime

## Importing into Eclipse

1. Open Eclipse
2. File → Import → Existing Projects into Workspace
3. Select the project directory
4. Configure project facets:
   - Java 11
   - Dynamic Web Module 5.0
5. Add required JARs to build path
6. Configure server runtime

## Running the Application

1. Start MySQL server
2. Start Tomcat server
3. Deploy the application
4. Access the application at: `http://localhost:8080/happyfeets`

## Default Admin Credentials

- Username: admin
- Password: admin123

## Features in Detail

### User Features
- Registration and login
- Browse tour packages
- Book tours
- View booking history
- Update profile

### Admin Features
- Manage tour packages
- View all bookings
- Manage users
- Generate reports

## Security Features

- Password hashing
- Session management
- Input validation
- SQL injection prevention
- XSS protection

## Error Handling

- Custom error pages
- Logging
- User-friendly error messages

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

