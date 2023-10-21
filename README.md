# SoundSphere

CodePath WEB103 Final Project

Designed and developed by: [Jerry Shi, Donald Antonio Young]

🔗 Link to deployed app:

## About

### Description and Purpose

SoundSphere is a client-database web application that facilitates a platform where artists can connect with fans, and fans with artists. With recent changes in ownership for Bandcamp impacting the way it operates, we recognize an opportunity to provide a valuable service to both content creators and fans alike. Accordingly, with SoundSphere artists will be able to upload their discography and details for fans to purchase. With the transactional data that's collected, SoundSphere will have the opportunity to provide artists with the personal analytics they need to build their business, and more effectively connect with the people that love their work. Furthermore, this transactional data can be used by the SoundSphere platform to generate editorial content and make recommendations to fans looking for more of what they enjoy. For content creators, SoundSphere has the additional opportunity to offer a more equitable transaction rate than Bandcamp offers. Additionally, for employees, SoundSphere presents an opportunity to pursue a line of work they are passionate about with the benefits of the labor union they collectively choose.

### Inspiration

Bandcamp.com is an online music distribution platform recently sold by Epic Games to Songtradr. Users have collectively spent over $1.19 billion via the Bandcamp client applications. This includes 14 million albums, 10 million tracks, 1.8 million vinyl records, and 100,000 t-shirts this year alone. As such, high systematization is needed to process these user-driven payments. Furthermore, a database driven backend is necessary to store the larger quantities of data, much of it being audio files, release information, album art, customer profiles, etc... The database driven backend, then, will track the Artist and their Releases. These Releases will have a set of Tracks, and once a specific Customer has found a release to purchase, they can place an Order. To track the number of orders a Release has received, it will be connected to ReleaseOrders, which will also be connected to Orders. This backend will prop up a large, ecommerce platform, and as such, it will handle a constant inflow of transactions warranting a database.

## Tech Stack

Frontend:
Next.js, React, Javascript

Backend:
Supabase

## Features
One to many relation: Each artist has many releases.
Many to many relation: Each release will be tied to orders which is the join table between releases and customers.
RESTful API design to allow for CRUD operations - Artist with releases, Customers with orders.
Reset function for database.
User can complete cart and check out as single page application.
404 site not found redirection.

Custom:
Checkout cart shows up as slide out.
User can sort artists by fields and filter.

### Fan registration

As a fan, I want to sign up so I can be able to catch up on the most recent releases of my favorite artists.

[gif goes here]

### Artist registration

As an artist, I want to sign up so I can be able to keep in touch with my audience.

[gif goes here]

### Fan profile creation

As a fan, I want to create and maintain a profile so I can showcase my personality and communicate with my favorite artists.

[gif goes here]

### Artist profile creation

As an artist, I want to create and maintain a profile so I can showcase my brand and communicate with my audience.

[gif goes here]

### Artist content upload

As an artist, I want to be able to upload my latest releases onto the web for my fans.

[gif goes here]

### Artist implements price change

As an artist, I want to be able to promote my releases with promotions so that I can sell more of my work.

[gif goes here]

### Artist's transaction data

As an artist, I want to be able to look through transaction data to figure out my largest markets and most loyal fans.

[gif goes here]

### Artist's discography view

As an artist, I want to be able to view my discography quickly and be able to share it to provide fans with a quick overview of my work.

[gif goes here]

### Fan downloads Artist content

As a fan, I want to be able to keep the content I paid for so I can keep my favorite work accessible on or offline.

[gif goes here]

### Fan view of their download collection

As a fan, I want to be able to quickly view which items I have downloaded already so I can know which items I have yet to download.

[gif goes here]

### Fans can search artists

As a fan, I want to search for artists to keep discovering new music.

[gif goes here]

### Fans can filter and sort artists by attributes

As a fan, I want to filter and sort artists so I can find artists I might enjoy.

[gif goes here]

### Fans view other Fan's profile

As a fan, I want to view other fans so I can connect with other users.

[gif goes here]

## Installation Instructions

[instructions go here]
