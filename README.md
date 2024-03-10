# DatabasePractise1

## Project Description

This project serves as an example of using a database in Java, utilizing the H2 Database. It is created for educational purposes and demonstrates basic database interaction without using the Spring framework or Maven.

## Prerequisites

Before running the project, make sure you have the following:

- Java Development Kit (JDK)
- IntelliJ IDEA or your preferred IDE

## Instructions for Running

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/k1fl1k/DatabasePractise1.git
    ```

2. Open the project in your chosen IDE (e.g., IntelliJ IDEA).

3. Run the main class `Main` to execute the program.

## Database Configuration

The project uses the H2 Database, and the database configuration is located in each `DAO` file. By default, the database uses the embedded file system.

```java
private Connection connect(){
    String url = "jdbc:h2:src/com/k1fl1k/dbpractice/persistance/database/storages_database";
    Connection conn = null;
    try {
        conn = DriverManager.getConnection(url);
    } catch (SQLException e) {
        System.out.println(e.getMessage());
    }
    return conn;
}
```

## Task

In this project, strive to apply SOLID and GRASP principles. You are creating a persistence layer – the data layer. 

1. Create a database.

2. Although there is no user interface, functionality should be verified in a "test class" with "test data."

## Contribution and Authorship

If you have ideas or would like to contribute to the project, please create a Pull Request or open a new Issue.

Author: [k1fl1k](https://github.com/k1fl1k)

## License

This project is distributed under the [MIT License](LICENSE).
