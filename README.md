# Ex09 Event Registration Web Application
## Date:15.10.2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
Home Page
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Festival - Saveetha Engineering College</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: linear-gradient(to bottom right, #f0f8ff, #e6ffe6);
      color: #333;
    }
    .header {
      background-color: #004d99;
      color: white;
      padding: 20px;
      text-align: center;
    }
    .header h1 {
      margin: 0;
      font-size: 28px;
    }
    .header p {
      margin: 5px 0;
      font-size: 16px;
    }
    .festival-title {
      text-align: center;
      font-size: 36px;
      color: green;
      margin: 30px 0;
    }
    .sports-illustration {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 20px;
      padding: 20px;
    }
    .sport-icon {
      width: 120px;
      height: 120px;
      background-color: #fff;
      border: 2px solid #ccc;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: bold;
      box-shadow: 2px 2px 10px rgba(0,0,0,0.1);
    }
    .buttons {
      text-align: center;
      margin: 40px 0;
    }
    .buttons button {
      background-color: #0073e6;
      color: white;
      border: none;
      padding: 12px 24px;
      margin: 10px;
      font-size: 16px;
      border-radius: 5px;
      cursor: pointer;
    }
    .buttons button:hover {
      background-color: #005bb5;
    }
  </style>
</head>
<body>

  <div class="header">
    <h1>Saveetha Engineering College</h1>
    <p>AUTONOMOUS | AFFILIATED TO ANNA UNIVERSITY</p>
  </div>

  <div class="festival-title">SPORTS FESTIVAL</div>

  <div class="sports-illustration">
    <div class="sport-icon">🏀 Basketball</div>
    <div class="sport-icon">⚽ Football</div>
    <div class="sport-icon">🎾 Tennis</div>
    <div class="sport-icon">🏇 Horse Riding</div>
    <div class="sport-icon">🏃 Running</div>
    <div class="sport-icon">🏐 Volleyball</div>
  </div>

  <div class="buttons">
    <button>LOGIN</button>
    <button>REGISTER</button>
  </div>

</body>
</html>

Page 2
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Day Events</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to bottom, #2c003e, #660000);
      color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 40px 20px;
    }

    h1 {
      color: yellow;
      font-size: 36px;
      margin-bottom: 30px;
      text-align: center;
      text-shadow: 2px 2px 5px black;
    }

    ul {
      list-style-type: none;
      padding: 0;
      max-width: 400px;
    }

    li {
      font-size: 24px;
      color: #00ccff;
      margin: 12px 0;
      position: relative;
      padding-left: 20px;
    }

    li::before {
      content: "*";
      position: absolute;
      left: 0;
      color: #ffcc00;
      font-weight: bold;
    }
  </style>
</head>
<body>

  <h1>SPORTS DAY EVENTS</h1>

  <ul>
    <li>CRICKET</li>
    <li>KABADDI</li>
    <li>BADMINTON</li>
    <li>TENNIS</li>
    <li>VOLLEY BALL</li>
    <li>FOOT BALL</li>
    <li>KHO-KHO</li>
    <li>ATHLETICS</li>
    <li>THROW BALL</li>
    <li>DOTCH BALL</li>
  </ul>

</body>
</html>

Page 3
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Event Registration Form</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(135deg, #ff66b2, #9933ff, #ffcc00, #00ccff);
      background-size: 400% 400%;
      animation: gradientShift 15s ease infinite;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .form-container {
      background-color: rgba(255, 255, 255, 0.1);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 20px rgba(0,0,0,0.3);
      width: 350px;
      color: purple;
    }

    h1 {
      text-align: center;
      font-size: 28px;
      color: limegreen;
      margin-bottom: 5px;
    }

    h3 {
      text-align: center;
      font-size: 16px;
      color: lightblue;
      margin-bottom: 20px;
    }

    label {
      display: block;
      margin: 10px 0 5px;
      font-weight: bold;
    }

    input, select {
      width: 100%;
      padding: 10px;
      border: none;
      border-radius: 8px;
      background-color: #ff66b2;
      color: purple;
      font-size: 14px;
    }

    .register-btn {
      margin-top: 20px;
      width: 100%;
      padding: 12px;
      background-color: yellow;
      color: purple;
      font-weight: bold;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }

    .register-btn:hover {
      background-color: gold;
    }
  </style>
</head>
<body>

  <div class="form-container">
    <h1>EVENT REGISTRATION FORM</h1>
    <h3>file details</h3>

    <form>
      <label for="name">FULL NAME:</label>
      <input type="text" id="name" name="name" required>

      <label for="gender">GENDER:</label>
      <select id="gender" name="gender" required>
        <option value="">Select</option>
        <option value="Male">Male</option>
        <option value="Female">Female</option>
        <option value="Other">Other</option>
      </select>

      <label for="age">AGE:</label>
      <input type="number" id="age" name="age" required>

      <label for="regno">REGISTER NO:</label>
      <input type="text" id="regno" name="regno" required>

      <label for="dept">DEPARTMENT:</label>
      <input type="text" id="dept" name="dept" required>

      <label for="mobile">MOBILE NO:</label>
      <input type="tel" id="mobile" name="mobile" required>

      <label for="event">EVENT:</label>
      <input type="text" id="event" name="event" required>

      <button class="register-btn" type="submit">REGISTER</button>
    </form>
  </div>

</body>
</html>

Page 4
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sports Invitation</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      background: radial-gradient(circle at center, #ff00cc, #6600ff, #ffcc00, #00ffff);
      background-size: 200% 200%;
      animation: explode 10s ease infinite;
      color: white;
      text-align: center;
    }

    @keyframes explode {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    .poster {
      background-color: rgba(0, 0, 0, 0.6);
      padding: 40px;
      border-radius: 20px;
      box-shadow: 0 0 30px rgba(255, 255, 255, 0.3);
      max-width: 600px;
    }

    .poster h1 {
      font-size: 32px;
      margin-bottom: 20px;
      color: #00ff99;
    }

    .poster p {
      font-size: 22px;
      line-height: 1.5;
      color: #ffccff;
    }
  </style>
</head>
<body>

  <div class="poster">
    <h1>Saveetha Engineering College</h1>
    <p><strong>We all eagerly waiting for you to participate in all the sport events occurred!</strong></p>
  </div>

</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot (45).png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
