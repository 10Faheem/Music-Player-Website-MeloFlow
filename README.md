# Music-Player-Website-MeloFlow

A website built in HTML and CSS, using PHP as the backend language with a small touch of JavaScript.

## Overview

This project is a music player website that allows users to browse, listen to, and manage music albums, artists, genres, and playlists. The website features a user-friendly interface with functionalities to create and manage playlists, view artist and album details, and much more.

## Features

- **User Authentication:** Users can sign up, log in, and manage their profiles.
- **Music Library:** Browse through a collection of albums, artists, and genres.
- **Playlists:** Create and manage playlists.
- **Song Playback:** Listen to songs with a built-in music player.
- **Search Functionality:** Search for songs, albums, and artists.
- **Responsive Design:** Optimized for both desktop and mobile devices.

## Database Structure

The project uses a SQL database to manage the data. Here is a brief overview of the database structure:

### Tables

#### album

- `album_id` (int, primary key)
- `Album_Name` (varchar)
- `Album_ReleaseDate` (date)

#### albumartist

- `Album_ID` (int, foreign key)
- `Artist_ID` (int, foreign key)

#### artist

- `Artist_ID` (int, primary key)
- `Artist_Name` (varchar)

#### artistgenre

- `Artist_ID` (int, foreign key)
- `Genre_ID` (int, foreign key)

#### genre

- `Genre_ID` (int, primary key)
- `Genre_Description` (varchar)
- `Genre_Name` (varchar)

#### lryiclanguage

- `Lyric_ID` (int, primary key)
- `Language_1` (varchar)
- `Language_2` (varchar)
- `Language_3` (varchar)

#### lyrics

- `Lyric_ID` (int, primary key)
- `Song_ID` (int, foreign key)

#### playlist

- `Playlist_ID` (int, primary key)
- `User_ID` (int, foreign key)
- `Playlist_Name` (varchar)
- `isPublic` (tinyint)

#### playlistsongs

- `Playlist_ID` (int, foreign key)
- `Song_ID` (int, foreign key)

#### songgenre

- `Song_ID` (int, foreign key)
- `Genre_ID` (int, foreign key)

#### songs

- `Song_ID` (int, primary key)
- `Release_Date` (date)
- `Song_title` (varchar)

#### subscription

- `Subscription_ID` (int, primary key)
- `Type` (varchar)
- `End_Date` (date)
- `Start_Date` (date)

#### user

- `User_ID` (int, primary key)
- `Subscription_ID` (int, foreign key)
- `First_Name` (varchar)
- `Last_Name` (varchar)
- `Password` (varchar)
- `Username` (varchar)

## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

- PHP
- MySQL
- Apache or any other web server
- Web browser

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/Music-Player-Website-MeloFlow.git
    ```

2. Import the SQL file into your database management system.

3. Update the database configuration in the project files.

4. Run the web server and open the project in your web browser.

## Usage

- Sign up or log in to access the music library.
- Browse through albums, artists, and genres.
- Create and manage playlists.
- Listen to songs using the built-in music player.
- Search for your favorite music.

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Contact

If you have any questions or need further assistance, feel free to contact me at: [fahimumer71@gmail.com](mailto:fahimumer71@gmail.com)

Project Link: [https://github.com/your-username/Music-Player-Website-MeloFlow](https://github.com/your-username/Music-Player-Website-MeloFlow)
