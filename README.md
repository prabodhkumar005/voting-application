# 🗳️ Voting Application

This is a backend application for a voting system where users can vote for candidates. It provides functionalities for user authentication, candidate management, and voting.

---

## 🚀 Features

- User sign up and login with Aadhar Card Number and password
- User can view the list of candidates
- User can vote for a candidate (only once)
- Admin can manage candidates (add, update, delete)
- Admin cannot vote

---

## 🛠️ Technologies Used

- Node.js  
- Express.js  
- MongoDB  
- JSON Web Tokens (JWT) for authentication

---

## 📡 API Endpoints

### 🔐 Authentication

- **Sign Up**  
  `POST /signup`  
  Sign up a new user

- **Login**  
  `POST /login`  
  Login an existing user

---

### 🧑‍💼 Candidates

- **Get Candidates**  
  `GET /candidates`  
  Retrieve the list of all candidates

- **Add Candidate** *(Admin only)*  
  `POST /candidates`  
  Add a new candidate

- **Update Candidate** *(Admin only)*  
  `PUT /candidates/:id`  
  Update a candidate by ID

- **Delete Candidate** *(Admin only)*  
  `DELETE /candidates/:id`  
  Delete a candidate by ID

---

### 🗳️ Voting

- **Get Vote Count**  
  `GET /candidates/vote/count`  
  Get the count of votes for each candidate

- **Vote for Candidate** *(User only)*  
  `POST /candidates/vote/:id`  
  Vote for a candidate (only once)

---

### 👤 User Profile

- **Get Profile**  
  `GET /users/profile`  
  Get user profile information

- **Change Password**  
  `PUT /users/profile/password`  
  Change user password

---

