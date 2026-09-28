# Salon Appointment Scheduler

Command-line appointment booking for a fictional salon, built for the freeCodeCamp **Relational Database** certification.

- `salon.sh` — Bash script: shows the services, validates the choice, finds or creates the customer by phone number, and books the appointment.
- `salon.sql` — PostgreSQL dump of the `salon` database (tables `services`, `customers`, `appointments`).

## Run

```bash
psql -U postgres < salon.sql
./salon.sh
```

The script connects as the `freecodecamp` user used in the course environment; change `PSQL` in `salon.sh` for your setup.

## What I would improve next

The SQL queries are built by inserting user input directly into strings, which is fine for a course exercise but unsafe in a real app. A production version would use parameterised queries.
