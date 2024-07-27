**Quote of the Day**
Overview
The Quote of the Day project is a simple web application that allows users to create, update, delete, and fetch quotes. It also provides a "Quote of the Day" feature, which displays a random quote from the database.

**Features**
Get Quote of the Day: Fetches a random quote from the database.
**Create a Quote:** Allows users to create a new quote with a name and quote text.
**Update a Quote:** Allows users to update an existing quote by its ID.
**Delete a Quote:** Allows users to delete a quote by its ID.
**Fetch Quotes by Name:** Fetches all quotes associated with a given name.

**Tech Stack**
Backend: Spring Boot
Frontend: HTML, CSS
Database: H2 (In-memory database for simplicity)

**Structure ---**

    ├── src
    │   ├── main
    │   │   ├── java
    │   │   │   └── org
    │   │   │       └── back
    │   │   │           └── end
    │   │   │               ├── DayOfMessageApplication.java
    │   │   │               ├── model
    │   │   │               │   └── Quote.java
    │   │   │               ├── repository
    │   │   │               │   └── QuoteRepository.java
    │   │   │               ├── rest
    │   │   │               │   └── controller
    │   │   │               │       └── QuoteOfTheDayRestController.java
    │   │   │               └── service
    │   │   │                   └── QuoteService.java
    │   │   └── resources
    │   └── test
    |
    ├── pom.xml
    ├── mvnw
    ├── mvnw.cmd
    └── README.md


**Getting Started** --

**Prerequisites**
Java 8 or higher
Maven

**Running the Application**
**Clone the repository:**
sh
Copy code
git clone https://github.com/your-username/day-of-message.git
cd day-of-message

Build the project using Maven:

sh
Copy code
mvn clean install
Run the application:

sh
Copy code
mvn spring-boot:run
Access the application at http://localhost:8080.

sh
Copy code
mvn test
API Endpoints
Get Quote of the Day: GET /quoteOfTheDay
Create a Quote: POST /quoteOfTheDay/create
Update a Quote: PUT /quoteOfTheDay/update
Delete a Quote: DELETE /quoteOfTheDay/{id}
Fetch Quotes by Name: GET /quoteOfTheDay/messageByName?name={name}

**Frontend**
The frontend is a simple HTML and CSS interface to interact with the backend API. It includes forms and buttons for each of the CRUD operations and the "Quote of the Day" feature.

**Customizing the Frontend**
You can customize the frontend by editing the index.html file located in the src/main/resources/static directory. The CSS is included inline for simplicity.

**Contributing**
Contributions are welcome! Please fork the repository and submit a pull request with your changes.
