A. Project Overvoew \n
this project is a java application that connects to the database, helping to work with various media content such as movies, series, episodes.  \n
Project has 4 entities:
1. Media content 
2. Movies
3. Series
4. Episodes
Media content is the base entity while others connect to it via foreign key 'media_id'. \n
This application follows OOP principles. Uses inheritance for shared behavior, polymorphism for unified access, encapsulation via private fields and getters/setters, custom exceptions hierarchy and CRUD operations via repositories.  \n
-----------
B. OOP Design Documentation
Media Content is an abstract class, while its subclasses are Movies, Series and Episodes.  \n
Interfaces and implemented methods - displayInfo(), IDB; \n
Aggregation - using a database and connecting to it. \n
Composition - usage of repositories. \n
Polymorphism examples: \n
List<Displayable> media = new ArrayList<>();  \n
media.add(movie); \n
media.add(series); \n
media.add(episode); \n
for (Displayable item : media) {  \n
    item.displayInfo();  \n
}  \n
Each object responds differently to the same method  \n

--------------
C. Controller
Example requests:  \n
1. movieService.getAll();
2. movieService.delete(2);

-------------------------
D. Instructions to run in java:
1. Compile: javac -cp .;postgresql.jar controller/Main.java
2. Run: java controller.Main

-----------
E. Reflection
I've learned how to properly connect to the database, also learned how to apply OOP principles. It was hard because this was my first experience and it was pretty confusing. 
Benefits of this multilayer design is that it makes it easier to maintain and change code, and maybe expand it. 
For JDBC - it provides ways to control SQL and update the database which makes it more convenient to work
