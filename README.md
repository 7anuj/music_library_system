Music Files Management System


Project Overview


The Music Files Management System is a database-driven application designed to efficiently manage digital audio files. Built using Python, MySQL (PyMySQL), and Tkinter, the system allows users to add, delete, and explore audio files based on multiple attributes such as genre, language, and album. It provides an intuitive and user-friendly graphical interface to organize and interact with a music collection.


Features


Add Songs: Users can input song details and store them in a MySQL database.
Delete Songs: Remove unwanted songs from the library.
Organize Songs: Sort and search songs based on genre, artist, language, or album.
View Songs: Browse and retrieve song details easily.
User-friendly GUI: Built with Tkinter for seamless interaction.
Efficient Data Management: Uses MySQL for structured data storage and retrieval.


Technologies Used


Python (Core logic & GUI handling)
MySQL (Database management)
Tkinter (Graphical User Interface)
PyMySQL (Database connection)


Database Structure


The system utilizes a relational database model, ensuring data integrity through normalization and functional dependencies.


Key Tables:


Tracks – Stores details like track title, artist, album, genre, language, release date, file location, and duration.
Artists – Maintains artist details such as name and origin.
Albums – Manages album-related information.
Genres – Categorizes tracks based on genre.
Languages – Stores the languages associated with tracks.


Functional Dependencies


Track ID -> Title, Artist ID, Album ID, Genre ID, Language ID, Release Date, File Location, Duration
Artist ID -> Artist Name, Origin
Album ID -> Album Title, Release Date, Genre ID, Artist ID
Genre ID -> Genre Name
Language ID -> Language Name


Installation & Setup


Install Dependencies:

pip install pymysql



Set up the MySQL Database:

Create a MySQL database and tables as per the schema provided in backend.py.
Update database connection details in the script.


Run the Application:

python main.py





File Structure


backend.py – Handles database interactions (CRUD operations).
main.py – Entry point of the application, initializes the GUI.
add.py – Provides an interface to add new music tracks.
delete.py – Enables track deletion from the library.
viewallsongs.py – Displays all tracks.
viewgenre.py – Filters songs by genre.
viewlanguages.py – Categorizes songs based on language.


Future Enhancements


User Profiles: Enable personalized recommendations and playlists.
Social Sharing: Share favorite tracks and playlists with others.
Advanced Search: Implement fuzzy search and metadata filtering.
Music Details Update: Allow updating artist and album details.
Streaming Service Integration: Connect with online music platforms for a richer experience.


References:


Tkinter Documentation
PyMySQL Documentation
