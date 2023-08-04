# Employee Registration Application (ASP.NET Core 6.0)
This is an employee registration application built on ASP.NET Core 6.0 web application using .NET 6.0 framework. The application allows users to create accounts, log in, and view employee profiles with pictures. Users can create their profile with one picture, which is downsized and stored in a MySQL database. Admin users have additional privileges, such as editing and deleting profiles, and managing users. Entity framework was not used.

# Features
* User Authentication & Authorization: Users can create accounts with hashed passwords and receive roles for authentication purposes. Cookie-based authorization is used to authenticate and authorize users.
* Profile Creation: Users can create their employee profile with information and a picture. The uploaded picture is automatically downsized and stored as byte[] in the MySQL database.
* Profile Display: Logged-in users can view cards with information and pictures of all the profiles created.
* Admin Panel: Admin users have access to additional features, such as edit and delete buttons on each profile. They can also manage all users and perform similar actions on their profiles.
* Password Security: All passwords are hashed before storing in the database using a secure hashing algorithm (bcrypt).
Database: The application uses MySQL as the database to store user accounts and employee profiles.
# Database
Database used is MySql with a premade data scheme, so to run this you would need to make your own scheme with data tables mimicking the objects user and profile and adjust the Sql queries in DbContext to match your tables names. You would also need to change the connection string in appsettings.json to match your own mysql servers database.
