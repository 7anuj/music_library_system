Music Files Management System


Project Overview


The Music Files Management System is a desktop application developed using Python, MySQL (PyMySQL), and Tkinter to efficiently manage digital audio files. This system enables users to add, delete, and organize songs in a structured database while providing an interactive graphical interface.


Features


Add Songs: Store song details such as title, artist, album, genre, and language.
Delete Songs: Remove songs from the database.
Organize Songs: Search and filter by genre, artist, language, or album.
View Songs: Retrieve song details with an easy-to-use interface.
Graphical User Interface: Built with Tkinter for an intuitive experience.
MySQL Database Integration: Ensures efficient storage and retrieval of music records.


Technologies Used


Python – Backend logic and GUI handling.
MySQL (PyMySQL) – Database management and queries.
Tkinter – Graphical interface for seamless interaction.


Database Structure


The database follows a relational model to maintain integrity and prevent redundancy.


Key Tables:


Tracks – Stores song details (title, artist, album, genre, language, release date, file location, duration).
Artists – Stores artist details (name, origin).
Albums – Contains album information.
Genres – Categorizes songs by genre.
Languages – Stores language details.


Functional Dependencies


Track ID -> Title, Artist ID, Album ID, Genre ID, Language ID, Release Date, File Location, Duration
Artist ID -> Artist Name, Origin
Album ID -> Album Title, Release Date, Genre ID, Artist ID
Genre ID -> Genre Name
Language ID -> Language Name


Installation & Setup


Install Dependencies:

pip install pymysql



Set up MySQL Database:

Create a database and tables using backend.py.
Update connection details in the script.


Run the Application:

python main.py





File Structure


backend.py – Handles database interactions (CRUD operations).
main.py – Initializes the GUI and runs the application.
add.py – Adds new tracks.
delete.py – Deletes existing tracks.
viewallsongs.py – Displays all songs.
viewgenre.py – Filters songs by genre.
viewlanguages.py – Categorizes tracks by language.


Future Enhancements


User Profiles: Enable personalized playlists and preferences.
Social Sharing: Share songs and playlists.
Advanced Search: Implement fuzzy search and metadata filtering.
Music Details Editing: Allow modifications to song details.
Streaming Service Integration: Connect with online music platforms.


References:


Tkinter Documentation
PyMySQL Documentation
