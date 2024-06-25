# RICELIPKA Directus POC
POC for RICELIPKA to run the latest version of Directus.

## MySQL 
Ensure MySQL is installed locally. If you need to import existing data, follow these steps:

1. Create a local MySQL DB:
```bash
mysql -u root -p
> CREATE DATABASE ricelipka_db;
> quit
```

2. Import Data (Optional):
```bash
mysql -u root -p ricelipka_db < backup_file.sql
```

## Getting Started
To get started with the project, follow these steps:

1. Install dependencies
```bash
npm install
```

2. Set up the Enviroment Variables
Copy the .env file
``` bash
cp .env.example .env
```

Edit the .env file with your configuration details.

## Directus
1. To bootstrap Directus and start the CMS:
```bash
npm run bootstrap
```

2. Start the CMS:
```bash
npm run start
```

Access Directus:

Visit http://localhost:8055 in your browser and log in using the credentials set in the `.env` file.