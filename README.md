# Gym Management System

## 📌 Description
This project is a simple database design and management system for a gym chain.  
The goal is to replace the outdated paper-based system and provide a digital solution to manage **gymnasiums, members, sessions, and coaches**.

The solution is based on an **Entity Relationship Diagram (ERD)** that models how the different entities interact with each other.

---

## 🏋️ Entities & Attributes

- **Gymnasium**
  - `gymnasium_id` (PK)
  - `name`
  - `address`
  - `telephone`

- **Member**
  - `member_id` (PK)
  - `last_name`
  - `first_name`
  - `address`
  - `date_of_birth`
  - `gender`

- **Session**
  - `session_id` (PK)
  - `sport_type`
  - `schedule`
  - `max_capacity` (default = 20)

- **Coach**
  - `coach_id` (PK)
  - `last_name`
  - `first_name`
  - `age`
  - `specialty`

---

## 🔗 Relationships
- A **Member** registers at **one Gymnasium**.  
- A **Member** can attend **many Sessions**, and a **Session** can have **many Members** (N:N).  
- A **Session** is hosted by **one Gymnasium**.  
- A **Session** can be led by up to **two Coaches** (1:2).  

---


