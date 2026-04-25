# CS-340 Client/Server Development — Portfolio Submission
**Student:** Kevin Simmons  
**Course:** CS-340 | Southern New Hampshire University

---

## Project Overview

This repository contains the artifacts from CS-340, including the CRUD Python module (Project One) and the Grazioso Salvare animal shelter dashboard (Project Two). The project connects a MongoDB database to an interactive web dashboard that helps Grazioso Salvare identify dogs suitable for rescue training based on breed, age, and rescue category.

---

## How do you write programs that are maintainable, readable, and adaptable?

I write maintainable and adaptable programs by separating concerns into reusable modules. In this course, the CRUD Python module (AnimalShelter class) was built as a standalone component that handled all database interactions — create, read, update, and delete — independently of the dashboard. This meant that when building Project Two, I simply imported the module and called its methods without rewriting any database logic.

The advantages of this approach were significant. The module was easy to test on its own, easy to debug, and easy to reuse. If the database changed (for example, switching from one collection to another), I only needed to update one file. In the future, this same CRUD module could be repurposed for any application that needs to interact with MongoDB — a mobile app backend, a REST API, or even another dashboard for a different organization.

---

## How do you approach a problem as a computer scientist?

I approached the Grazioso Salvare project by first understanding the client's requirements — they needed to filter rescue dogs by category (water rescue, mountain rescue, disaster tracking) and visualize the results. I then worked backward from that goal: what data was needed, how it should be queried, and how to display it.

This differed from previous assignments where the problem was more clearly defined and solutions were more straightforward. Here, I had to think about the end user's workflow and make design decisions about the dashboard layout, filter logic, and data presentation. In the future, I would continue using this requirements-first approach — understanding what the client needs before writing any code — and pair it with incremental testing to ensure each component works before connecting them.

---

## What do computer scientists do, and why does it matter?

Computer scientists solve real-world problems by designing systems that make information accessible, useful, and actionable. In this project, the work directly supported Grazioso Salvare's mission of training rescue animals. Without a database and dashboard, staff would have to manually sort through thousands of animal records to find suitable candidates — a slow and error-prone process.

By building a filtered, interactive dashboard backed by a MongoDB database, the organization can instantly identify the right dogs for each rescue category. This kind of work matters because it turns raw data into decisions, saving time and ultimately helping save lives through more effective rescue operations.

---

## Repository Contents

- `CRUD_Python_Module.py` — Reusable Python module for MongoDB CRUD operations
- `ProjectTwoDashboard.ipynb` — Jupyter Notebook dashboard for Grazioso Salvare
- `README.md` — Project documentation and reflection
