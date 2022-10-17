# Software Requirements

## Vision

### What is the vision of this product?

Buld an application that is a card collection portfolio for all users who are interested in trading card games. Users can search all cards through a (3rd party Dataset) and add any of their choosing to their portfolio. They can then set them into their portfolio to view and remove if desired

### What pain point does this project solve?

This solves the isssue of collecting cards that you own and trying to learn about every feature of each card. This can also help you to easily access cards that you have recently added to your collection into a portfolio of your own without having to manually add all of the featured detatils yourself, effectively saving you plenty time.

### Why should we care about your product?

 If you are a fan of any kind of card games (which can count for about 80% of the word), our algoritm an implementation for this project can be used for your own card games, maximizing opportunities to create more order and fun for the games that you love.

## Scope

The web app wil let users search apis for

IN - What will your product do
 Multiple Users will only be able to read your portfolio.
 The application will prompt the user to sign in to verify its acccout and ensure the user is authorized
 The application will establish a many-to-many validation for adding cards, removing them, and verifyiing them.
The user will be able to filter such cards by orientation of color, types, mana and power.

OUT - What will your product not do
 Multiple Users will not be able to interfere with your own account by making edits, adding new data, or removing data.
 This application will not run in the front end (only within the server/backend)

### Minimum Viable Product

MVP:
0Auth: User needs to have an account
Role Based Access control
Can add a validated card to your portfolio
Many-to-many validation
User can POTENTIALLY look at users’ info, only with read role
Once deployed, can be moved to SQL Database

Stretch Goals:
Deck Builder? Cards added can be placed into decks
Set rules to the deck
User can only own up to # of cards
Open API Discord Bot
(Optional:) User can import data (their cards) either import a single card or a JSON object with as many cards as you’d like (array of card titles)
Use Trulioo for text message
A person can come into the server, must be a verified player by passing a test of 10 indentifying questions in order to be an official user. Once the person passes only then are they given a key/invitation link to sign up with their own account.

## Functional Requirements

An admin/developer can create and delete user accounts
An admin/developer can update the card database by using a lambda function to parse new data and feed data into the databse
A user can update their profile information
A user can search all of the cards in the database
A user can add card(s) to their portfolio
A user can remove card(s) to their portfolio
A user can read/view other users portfolio(s)

### Data Flow

From the time the user begins using the app:

![uml](UntappedIsland.png)

To the time the user is done with the app:

## Non-Functional Requirements

Security
0Auth is implemented successfully.
Hash: User can only log in by key or invitation link sent by admin (limits large amount of users and adds another security level.
Useability
 Data is shown in the terminal once the user creates/logs into their acccount.
User can log in and log out without any delay.
Little to no bugs shown in the data provided to the user.
 Testability
 At least 80% of all tests are passing
