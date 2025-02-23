# World Seed Data Repository

## Overview
This repository contains a comprehensive dataset of global geographical entities, including countries, states, cities, regions, and subregions. The data is structured and formatted for seamless integration with Flyway for database migrations and seeding.

## Features
- **Complete dataset**: Includes cleaned and structured data for countries, states, cities, regions, and subregions.
- **Flyway integration**: Ready-to-use SQL files for automatic database migration and seeding.
- **Consistent formatting**: Data follows a standardized format to ensure easy integration.
- **Scalable and maintainable**: Designed for efficient updates and expansions.

## Repository Structure
```
|-- migrations/
|   |-- V1.0.0__geo_tables.sql
|   |-- V1.0.1__seed_cities.sql
|   |-- V1.0.2__seed_cities.sql
|   |-- V1.0.3__seed_cities.sql
|   |-- V1.0.4__seed_cities.sql
|   |-- V1.0.5__seed_cities.sql
|   |-- V1.0.6__seed_cities.sql
|   |-- V1.0.7__seed_cities.sql
|   |-- V1.0.8__seed_cities.sql
|   |-- V1.0.9__seed_cities.sql
|   |-- V1.0.10__seed_cities.sql
|   |-- V1.0.11__seed_cities.sql
|   |-- V1.0.12__seed_cities.sql
|   |-- V1.0.13__seed_cities.sql
|   |-- V1.0.14__seed_cities.sql
|   |-- V1.0.15__seed_cities.sql
|   |-- V1.0.16__seed_cities.sql
|   |-- V1.0.17__seed_countries.sql
|   |-- V1.0.18__seed_regions.sql
|   |-- V1.0.19__seed_states.sql
|   |-- V1.0.20__seed_subregions.sql

|   |-- V5__insert_states.sql
|   |-- V6__insert_cities.sql
|-- README.md
```

- **migrations/**: Contains Flyway migration scripts in chronological order.
- **V1.0.0__geo_tables.sql**: Creates the necessary tables for the dataset.
- **V1.0.1__seed_cities.sql - V1.0.20__seed_subregions.sql**: Inserts data for different geographical levels.

## Prerequisites
- **Database**: PostgreSQL (or compatible database supported by Flyway)
- **Flyway**: Ensure Flyway is installed and configured

## Installation & Usage
### 1. Clone the repository
```sh
git clone https://github.com/your-repo/world-seed-data.git
cd world-seed-data
```

### 2. Configure Flyway
Update your Flyway configuration (`flyway.conf`) to point to your database:
```properties
flyway.url=jdbc:postgresql://localhost:5432/your_database
flyway.user=your_username
flyway.password=your_password
```

### 3. Run Flyway Migrations
```sh
flyway migrate
```
This will create the necessary tables and seed them with the world dataset.

## Contribution
Contributions are welcome! If you find missing data or errors, feel free to open an issue or submit a pull request.

## License
This dataset is released under the MIT License. Feel free to use it in your projects while giving proper attribution.

## Contact
For any questions or issues, please open an issue on GitHub.

---

Enjoy using the World Seed Data repository! 🌍🚀

