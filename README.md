# YouTube Clone — Java & JavaFX

A YouTube-inspired desktop application built with **Java**, **JavaFX**, and **PostgreSQL** as the final project for an **Advanced Programming** course at Shahid Beheshti University.

The project was developed as a team and focuses on implementing the core concepts of a video-sharing platform, including authentication, video management, playback, comments, likes, subscriptions, search, and database-backed client-server communication.

> **Project type:** University team project
> **Course:** Advanced Programming
> **Platform:** Desktop
> **Primary technologies:** Java, JavaFX, PostgreSQL

---

## Overview

The project recreates the core experience of a video-sharing platform similar to YouTube as a Java desktop application.

Users can create accounts, upload and watch videos, interact with videos through comments and likes/dislikes, subscribe to channels, and search for video content.

The application uses **JavaFX** for the graphical user interface and **PostgreSQL** for persistent data storage, with client-server communication connecting the application components.

---

## Features

### User Authentication

* User registration
* User login
* Individual user accounts

### Video Management

* Upload videos
* Add video titles
* Add descriptions
* Add tags
* Browse available videos

### Video Playback

* Play videos
* Pause videos
* Seek through videos

### Social Features

* Comment on videos
* Like/dislike videos
* Subscribe to channels

### Search

Users can search for videos based on:

* Title
* Description
* Tags

### Database

The application uses PostgreSQL for persistent storage and includes a relational database design represented by an Entity-Relationship Diagram (ERD).

---

## Technology Stack

| Technology | Purpose                                  |
| ---------- | ---------------------------------------- |
| Java       | Core application and backend development |
| JavaFX     | Desktop graphical user interface         |
| PostgreSQL | Relational database                      |
| Maven      | Project and dependency management        |

---

## Architecture

The project follows a client-server structure:

```text
┌──────────────────────┐
│      JavaFX Client   │
│                      │
│  User Interface      │
│  Video Interaction   │
│  User Interaction    │
└──────────┬───────────┘
           │
           │ Client-Server Communication
           ▼
┌──────────────────────┐
│       Server         │
│                      │
│  Application Logic   │
│  Data Processing     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│      PostgreSQL      │
│                      │
│  Users               │
│  Videos              │
│  Comments            │
│  Relationships       │
│  Other application   │
│  data                │
└──────────────────────┘
```

The repository also includes both a **UML class diagram** and an **ERD** documenting the application's object model and database structure.

---

## Database Design

PostgreSQL is used as the project's persistent database.

The repository includes the database SQL script:

```text
YoutubeDB.sql
```

and an ERD describing the relationships between the database entities.

The database layer supports the application's main concepts, including users, videos, interactions, and subscriptions.

---

## Project Documentation

The repository contains architectural documentation alongside the source code:

* `ModelClassesUML.png` — UML diagram of the model classes
* `ERD.png` — Entity-Relationship Diagram
* `YoutubeDB.sql` — PostgreSQL database definition/data
* `YoutubeDemo.mp4` — Project demonstration

These artifacts document both the software structure and the database design.

---

## Team Contributions

This was a collaborative university project.

### Ali Taherzadeh

**Client-server communication and data flow**

Responsible for implementing and handling the communication between the application components and ensuring efficient data flow between the client and server.

### Mohammad Sajjad Zanganeh

**JavaFX interface and view-controller layer**

Responsible for the JavaFX view-controller relationships and responsive UI implementation.

### Hamed Pooraghniaei

**Backend API and database**

Responsible for backend API development and database management.

---

## Course Context

This project was developed as the **final project of the Advanced Programming course** at **Shahid Beheshti University**.

The goal was to apply object-oriented programming and advanced Java concepts to a larger, collaborative software project rather than a small isolated programming exercise.

The project was developed before the widespread use of AI-assisted programming tools.

---

## What I Learned

Through this project, I gained practical experience with:

* Java application development
* Object-Oriented Programming
* JavaFX
* Desktop GUI development
* Client-server architecture
* Inter-component communication
* Data flow between application layers
* PostgreSQL
* Relational database design
* ER diagrams
* UML class diagrams
* Maven
* Collaborative software development

---

## Demo

A recorded demonstration of the application is included in the repository:

**`YoutubeDemo.mp4`**

The demonstration covers major application functionality including:

* User authentication
* Video upload
* Video playback
* Comments
* Subscriptions

---

## Repository Structure

The project includes:

```text
Youtube-Clone/
├── src/
│   └── main/
├── .mvn/
│   └── wrapper/
├── ERD.png
├── ModelClassesUML.png
├── YoutubeDB.sql
├── YoutubeDemo.mp4
├── pom.xml
├── mvnw
├── mvnw.cmd
└── README.md
```

---

## Educational Project

This project is an educational implementation inspired by the core functionality of YouTube.

It is **not affiliated with or endorsed by YouTube or Google** and is not intended to reproduce the production architecture or infrastructure of YouTube.

---

## License

No license has been specified for this project.
