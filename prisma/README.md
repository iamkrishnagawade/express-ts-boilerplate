# Prisma Setup Guide

This document explains the Prisma setup in this project.

## Quick Start

Run these commands to initialize and apply your database schema:

1. Initialize Prisma and create the initial migration:
   ```bash
   npx prisma migrate dev --name init
   ```

2. (Optional) If you need to reset your database and start fresh:
   ```bash
   npx prisma migrate reset
   ```

3. `npx prisma studio` -> GUI for database. (Runs on localhost:51212 by default)

4. `npx prisma generate` -> Generate prisma client. (Runs automatically after `npx prisma migrate dev`)

5. `npx prisma db push` -> Push schema to database. (Runs automatically after `npx prisma migrate dev`)

6. `npx prisma db seed` -> Seed database. (Runs automatically after `npx prisma migrate dev`)

## Prisma Commands

- **Generate client**: `npx prisma generate` (run after schema changes)
- **Apply migrations**: `npx prisma migrate dev`
- **Reset database**: `npx prisma migrate reset`
- **Studio** (GUI): `npx prisma studio`
- **Seed database**: `npx prisma db seed`
