**Phase 1**
**Dariush and Darius** will make an sql table for the Lakers, Rockets, Thunder, Spurs, and Timberwolves. Store player and game information of the last 5 years
**Dariush and Darius** will make find an API key and will work try to get data for the stock market AMD, and then Store the AMD data in our database

**Justin and Dariush** will attempt to Web Scrape into our database the stats of ever player for the last 5 years into our database.
**Justin** will create and manage the project's API keys and JWT secrets. You will set up a safe way for the team to use API keys without putting them directly in the code. You will ensure that no one will use our database without those codes. You will Secure the database and decide who/what is allowed to access it. You will also protect the web-scraping process and outside connections. Begin setting up security logging so we can see failed or suspicious requests. Test the database and APIs for obvious security problems.

**Dariush** will add my info into a private data base of my stocks into it









## Phase 1 — Build the Data Foundation

The purpose of Phase 1 is to prove that we can **collect real data, store it correctly, protect it, and retrieve it through our system.**

We are **not building prediction models yet**.

### Dariush and Darius

* Create SQL tables for the **Lakers, Rockets, Thunder, Spurs, and Timberwolves**.
* Store player and game information from the **last 5 years**.
* Decide which statistics we need to save for future predictions.
* Find a stock-market data source/API for **AMD**.
* Successfully collect AMD stock information.
* Store the AMD information inside the database.
* Clean and organize the basketball and stock data before storing it.
* Check for missing, incorrect, or duplicate data.

### Justin and Dariush

* Attempt to web scrape player statistics from the **last 5 years** for the five selected NBA teams.
* Send the collected information into the database.
* Make sure the scraper does not create duplicate records.
* Make sure the scraper can recover from failed requests or bad information.
* Record where the scraped information came from and when it was collected.

### Justin — Security

Justin will build the first version of the project's security system.

#### Application Security

* Review how the application communicates with the database.
* Make sure private information is not exposed through the application.
* Check for obvious security weaknesses.

#### Identity & Access Management

* Create and manage the project's JWT secrets.
* Create a system that determines who is allowed to access protected parts of the project.
* Prepare the foundation for different types of users and permissions later.

#### Network Security

* Protect communication between the application, database, APIs, and web scrapers.
* Decide which parts of the system should be allowed to communicate with each other.
* Prevent unnecessary outside access to the database.

#### Security Operations / Detection

* Begin creating security logs.
* Record failed login/access attempts.
* Record suspicious API requests.
* Record unusual attempts to access the database.
* Make it possible for the team to review security events.

#### Data Security

* Protect private user information.
* Make sure sensitive information is not stored in plain text when it should be protected.
* Separate public sports/stock data from private user information.

#### DevSecOps

* Make sure API keys, JWT secrets, passwords, and other secrets are **never committed directly to GitHub**.
* Create a safe method for the team to use secrets while developing the project.
* Add basic security checks to the development process.

#### Penetration Testing / Security Testing

* Try to access protected information without proper permission.
* Test what happens when an invalid API key or token is used.
* Test whether someone can access database information they should not see.
* Document any weaknesses that are discovered.

#### Privacy Engineering

* Identify which information in the project is public and which information is private.
* Make sure private financial information is only available to the correct user.
* Begin documenting what personal information the platform stores.

#### API Security Engineering

* Secure API endpoints.
* Require proper authentication for protected endpoints.
* Add rate limits where necessary.
* Make sure invalid requests are rejected safely.

#### Database Engineering

* Work with Dariush and Darius on the database structure.
* Create database users and permissions.
* Prevent people from directly accessing information they are not authorized to view.
* Help design the private financial-data portion of the database.

### Dariush — Technical Lead

Dariush will lead Phase 1 and help both Justin and Darius whenever needed.

#### Backend Engineering

* Build the first backend connection to the database.
* Create the first endpoints that retrieve basketball and stock information.
* Connect the web-scraped information to the backend.

#### System Architecture

* Decide how the database, backend, web scraper, stock API, and security system communicate.
* Keep the project separated into understandable parts so it can grow later.

#### Cybersecurity

* Work with Justin to integrate the security system into the application.
* Make sure security is included while features are being built rather than added afterward.

#### Networking

* Build the communication between the backend, database, APIs, and data collectors.
* Learn how requests travel through the system.
* Help Justin secure those connections.

#### Data Engineering

* Build the process that takes collected information and moves it into the database.
* Make sure basketball and stock information follow consistent formats.

#### Database Engineering

* Design the overall database structure with Darius and Justin.
* Decide how tables connect to each other.
* Build the private financial-data portion of the database.

#### Cloud / DevOps

* Prepare the project so it can eventually be deployed.
* Organize development and production settings separately.
* Help establish safe environment configuration for the team.

#### Technical Leadership

* Assign tasks.
* Review everyone's work.
* Help Darius learn.
* Help Justin integrate his security work.
* Make sure everyone's part connects to the same project.
* Maintain the overall direction of the system.

#### Machine Learning Engineering

Machine learning will **not be built during Phase 1**.

Instead, Dariush will make sure the data being collected now is useful enough to eventually train:

* NBA player-stat prediction models
* Sports prop prediction models
* Stock-market prediction models

### Darius — Product & Data

Because Darius is new to coding, Phase 1 will also introduce him to development through real project work.

#### Product Management

* Help decide which statistics and stock information are actually useful to users.
* Keep track of what Phase 1 needs to accomplish.
* Help document future feature ideas.

#### User Experience / UX

* Think about how users should eventually search for players, teams, and stocks.
* Sketch how the sports and stock sections could be organized.
* Test early versions of the application from a normal user's perspective.

#### Data Collection

* Work with Dariush to find basketball and stock information.
* Research possible data sources.
* Verify collected information against trusted sources.

#### Data Cleaning

* Look for missing values.
* Find duplicates.
* Fix inconsistent player/team names.
* Help make dates and statistics consistent.

#### SQL / Database Work

* Help create the first tables.
* Learn how to insert information.
* Learn how to retrieve information.
* Learn how tables relate to each other.
* Gradually take responsibility for more database work as the project grows.

---

# Private Financial Database

Dariush will also create the first **private-user-data test case** using his own stock information.

This information should be stored separately from public stock-market information.

For example:

**Public AMD data**

* Current price
* Historical prices
* Volume
* Market information

**Private Dariush data**

* Shares owned
* Purchase price
* Amount invested
* Personal watchlist information

Justin and Dariush will make sure that this private information **cannot be retrieved without the correct authorization**.

This gives us a real reason to implement security instead of creating fake security features just for the résumé.

---

# Phase 1 Final Test

Phase 1 is complete when we can demonstrate all of this:

1. We have NBA player/game data for our five selected teams.
2. We have historical information stored in SQL.
3. We can collect AMD stock-market data.
4. AMD data is being stored in the database.
5. Our web scraper can collect basketball information and insert it into the database.
6. The backend can retrieve stored information.
7. API keys and JWT secrets are not exposed in the source code.
8. The database rejects unauthorized access.
9. Security events are being logged.
10. Dariush's private stock information cannot be viewed without proper authorization.
11. Darius can perform basic data collection, cleaning, and SQL tasks.
12. All three team members can explain how their part connects to the complete system.

## Phase 1 Architecture

**Sports / Stock Sources**
↓
**Darius + Dariush — Data Collection & Cleaning**
↓
**Justin + Dariush — APIs / Web Scraping**
↓
**SQL Database**
↓
**Justin — Security & Access Control**
↓
**Dariush — Backend**
↓
**Future Frontend**

Phase 1 gives us the foundation required for the prediction systems we will build later.
