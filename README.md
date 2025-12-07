🎵 Soundify – Console-Based Music Player (C++ & SFML)

Soundify is a fully-featured console music player built in C++, powered by the SFML Audio library. It allows users to play songs, manage playlists, browse genres, search tracks, and maintain a recently played history — all through an interactive terminal UI.

🚀 Features
🎶 Music Playback

Play, pause, resume, and stop songs

See real-time playback duration

Loop songs on/off

Skip forward/backward between songs

Uses SFML Audio for smooth music playback

📚 Song Management

Load and store songs from external files

Search songs by name

Display all songs with metadata (name, artist, genre)

📂 Playlist System

Create and delete playlists

Add/remove songs from playlists

Save playlist data to files

Play songs directly from any playlist

Maintains a Recently Played playlist (auto-updated)

🌲 Genre Browsing (Binary Tree Based)

Genre hierarchy stored in a complete binary tree

Navigate genre nodes to select sub-genres

Auto-generate playlists of all songs matching a selected genre

🗃️ Data Structures Used

This project showcases heavy use of custom data structures:

Hash Table for fast song lookup

Doubly Linked List for playlists

Stack for recently played history

Queue for tree insertion

Binary Tree for genre navigation

Linked Lists for hash collisions

🖥️ Console UI

Personalized ASCII logo

Centered UI elements

Keyboard-controls for live playback

User-friendly menu system

🛠️ Technologies Used

C++ (OOP + Data Structures)

SFML (Simple and Fast Multimedia Library) – Audio Module

Windows Console API (Windows.h)

Dynamic Memory Management

File I/O for persistent storage

📁 Project Structure

Song — container for song metadata

Hash / HashNode — hash table to store songs

Playlist / PNode — doubly linked list managing playlists

Tree / TNode — binary tree storing genre categories

Stack — managing recently played list

Queue — tree insertion

playMusic() — playback controller

loadData() — loads all songs on startup

📄 How It Works

songs.txt loads all music data

The program hashes and stores each song

The user navigates menus to:

Search songs

Play songs

Manage playlists

Explore genres

Playback is live-controlled using keyboard input

Recently Played list automatically updates

▶️ Requirements

SFML 2.5+

C++17 or higher

Windows OS (due to conio.h and Windows.h)

Place songs and metadata in the correct folder structure:

D:\songs\
  ├── songs.txt
  ├── Playlists.txt
  ├── Recently Played.txt
  ├── <playlist>.txt
  └── audio files (.wav/.ogg/.mp3 supported by SFML)

📌 Future Improvements

GUI version using SFML Graphics

Cross-platform support

Better hashing for names

Replace raw pointers with smart pointers

JSON-based storage system
