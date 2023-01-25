<h1 align="center">Habits API</h1>

<h3 align="center">Índice</h3>

<p align="center">
  <a href="#ℹ-about">About</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-documentation">Documentation</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-technologies">Technologies</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-see-more">See more</a>
</p>

## ℹ About

<p>Habits API is an application that provides a REST API to Habits Web/Mobile application.</p>

## 📘 Documentation

### Habits

#### Create a habit

`POST /habits`

| Field    | Type     | Description 
-----------|----------|--------------------------------
| title    | `string`   | Habit title
| weekDays | `number[]` | Frequency of the habit (0 to 6)

#### Toggle a habit progress (complete/uncomplete)

`PATCH /habits/{id}/toggle`

| Field    | Type     | Description 
-----------|----------|--------------------------------
| id       | `string`   | Habit id

### Summary

#### Get a summary of all day habits

`GET /summary`

### Day

#### Get details of a habit day

`GET /day?date={date}`

| Field    | Type     | Description 
-----------|----------|--------------------------------
| date     | `string` | Habit day that you want to search. Format example: 2023-01-23T14:00:00.000z

## ⚙ Technologies

<p>This app was made using this technologies:</p>

- Node.js
- Fastify
- zod
- Prisma
- SQLite

## ➕ See more

- [Habit Tracker Mobile](https://github.com/erick-menezes/habit-tracker-mobile)
- [Habit Tracker Web](https://github.com/erick-menezes/habit-tracker-web)
