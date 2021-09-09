   # Django GraphQL

  Instruction for setting up GraphQL in a Django Project.

  [TutorialPOints](https://www.tutorialspoint.com/index.html)
  
  ---
  **Table of content:**

  1. [why GraphQL?](#why-graphql)
  1. [Graphene Installation](#graphene-installation)
  2. Creating Schemas
  3. Using GraphiQL
  
  ## Why GraphQL
  
  - Get only the data that you want 
  - Easier to manage endpoints
    
  ## Graphene Installation

 Install Graphene: `pip install django_graphene`
 
 ## Creating Schemas

 ```java code 
 public static void main(String[] args) {
    Connection conn = null;
    Statement stmt = null;
    try {
        Class.forName("org.postgresql.Driver");

        System.out.println("Connecting to database...");
        conn = DriverManager.getConnection(DB_URL, USER, PASS);

        System.out.println("Creating Schema...");
        stmt = conn.createStatement();

        String sql = "CREATE SCHEMA centro";
        stmt.executeUpdate(sql);
        System.out.println("Schema created successfully...");
    } catch (SQLException se) {
        se.printStackTrace();
    } catch (Exception e) {
        e.printStackTrace();
    } finally {
        try {
            if (stmt != null) {
                stmt.close();
            }
        } catch (SQLException se2) {
        }
        try {
            if (conn != null) {
                conn.close();
            }
        } catch (SQLException se) {
            se.printStackTrace();
        }
    }
    
 ```

 ---
 >Steve Jobs was a charismatic pioneer of the personal computer era. With Steve Wozniak, Jobs founded Apple Inc. in 1976 and transformed the company into a world leader in telecommunications. Widely considered a visionary and a genius, he oversaw the launch of such revolutionary products as the iPod and the iPhone.
 >
 >> It is easy to handle.   

 --- *Stve Jobs*

 [![TutorialPointslogo](./tplogo.png)](https://www.tutorialspoint.com/index.htm)

-[x] Task #1

-[ ] Task #2