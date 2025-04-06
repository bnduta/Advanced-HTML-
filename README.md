<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Advanced HTML5 Elements and Forms</title>
  <style>
    /* Basic styling for table */
    table {
      width: 100%;
      border-collapse: collapse;
      margin-bottom: 20px;
    }
    th, td {
      border: 1px solid #ddd;
      padding: 8px;
    }
    th {
      background-color: #f2f2f2;
      text-align: left;
    }
    /* Styling for form */
    form {
      max-width: 600px;
      margin: 0 auto;
    }
    label {
      display: block;
      margin: 10px 0 5px;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-bottom: 10px;
    }
    fieldset {
      margin-bottom: 10px;
    }
    legend {
      font-weight: bold;
    }
    input[type="submit"] {
      background-color: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
    }
    input[type="submit"]:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <!-- Ordered List with Roman Numerals -->
  <section>
    <h2>Ordered List with Roman Numerals</h2>
    <ol type="I">
      <li>First item</li>
      <li>Second item</li>
      <li>Third item</li>
    </ol>
  </section>

  <!-- External Image from Pexels -->
  <section>
    <h2>External Image from Pexels</h2>
    <img src="https://www.pexels.com/photo/your-image.jpg" alt="Description of image">
  </section>

  <!-- Table of Contacts -->
  <section>
    <h2>Contact List</h2>
    <table>
      <thead>
        <tr>
          <th>Name</th>
          <th>Address</th>
          <th>Mobile</th>
          <th>Email</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>John Kim</td>
          <td>Kasarani</td>
          <td>0797123456</td>
          <td>john.kim@example.com</td>
        </tr>
        <tr>
          <td>Jane Wangui</td>
          <td>Metropolis</td>
          <td>077654321</td>
          <td>jane.wangui@example.com</td>
        </tr>
        <tr>
          <td>Emily Johnson</td>
          <td>Juja</td>
          <td>0722334455</td>
          <td>emily.johnson@example.com</td>
        </tr>
      </tbody>
    </table>
  </section>

  <!-- Registration Form -->
  <section>
    <h2>Registration Form</h2>
    <form action="submit_form.php" method="post">
      <!-- Name Field -->
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" placeholder="Enter your full name" required>

      <!-- Email Field -->
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" placeholder="Enter your email" required>

      <!-- Password Field -->
      <label for="password">Password:</label>
      <input type="password" id="password" name="password" placeholder="Enter your password" required>

      <!-- Date of Birth Field -->
      <label for="dob">Date of Birth:</label>
      <input type="date" id="dob" name="dob" required>

      <!-- Dropdown Field -->
      <label for="country">Country:</label>
      <select id="country" name="country" required>
        <option value="">Select your country</option>
        <option value="usa">United States</option>
        <option value="canada">Canada</option>
        <option value="uk">United Kingdom</option>
        <option value="australia">Australia</option>
        <option value="kenya">Kenya</option>
        <!-- Add more options as needed -->
      </select>

      <!-- Radio Buttons -->
      <fieldset>
        <legend>Gender:</legend>
        <input type="radio" id="male" name="gender" value="male" required>
        <label for="male">Male</label>
        <input type="radio" id="female" name="gender" value="female" required>
        <label for="female">Female</label>
        <input type="radio" id="other" name="gender" value="other" required>
        <label for="other">Other</label>
      </fieldset>

      <!-- Checkboxes -->
      <fieldset>
        <legend>Interests:</legend>
        <input type="checkbox" id="sports" name="interests" value="sports">
        <label for="sports">Sports</label>
        <input type="checkbox" id="music" name="interests" value="music">
        <label for="music">Music</label>
        <input type="checkbox" id="movies" name="interests" value="movies">
        <label for="movies">Movies</label>
        <!-- Add more checkboxes as needed -->
      </fieldset>

      <!-- Submit Button -->
      <input type="submit" value="Register">
    </form>
  </section>

</body>
</html>
