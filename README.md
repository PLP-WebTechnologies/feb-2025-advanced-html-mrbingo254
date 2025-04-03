# Advanced HTML5 Elements and Forms

## Objectives
Implement HTML5 images, lists, tables, forms and input types.
Use form validation attributes.
Apply multimedia elements such as audio and video.

## Instructions

- Create an index.html file.
- Add an ordered list with roman numerals
- Add an external image from pexels.com
- Add a table of 5 contacts with; name, address, mobile and emails
- Add a registration form

>[!NOTE]
>  The registration form should have:
>- Name, email, password, and date fields.
>- A dropdown, radio buttons, and checkboxes.
>- Proper labels and placeholders.
>- Required fields and validation attributes.
>- Ensure proper indentation and commenting.
 
# Tasks
- Create a well-structured HTML5 document.
- Ensure semantic correctness.

Happy Coding! 💻✨

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multimedia Webpage</title>
    <style>
        /* Basic styling for layout */
        body {
            font-family: Arial, sans-serif;
            max-width: 800px;
            margin: 0 auto;
            padding: 20px;
        }
        table {
            border-collapse: collapse;
            width: 100%;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: left;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <h1>Multimedia Experience</h1>
    </header>

    <!-- Audio Element -->
    <section>
        <h2>Listen to Music</h2>
        <audio controls>
            <source src="https://www.w3schools.com/html/horse.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </section>

    <!-- Video Element -->
    <section>
        <h2>Watch a Video</h2>
        <video controls width="400">
            <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
            Your browser does not support the video element.
        </video>
    </section>

    <!-- Embedded Image -->
    <section>
        <h2>Featured Image</h2>
        <img src="https://via.placeholder.com/300x200" alt="Sample Image" width="300" height="200">
    </section>

    <!-- Registration Form with Validation -->
    <section>
        <h2>Register Here</h2>
        <form>
            <fieldset>
                <legend>User Information</legend>
                
                <label for="username">Username:</label>
                <input type="text" id="username" name="username" required minlength="3" placeholder="Enter username">
                <br><br>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required placeholder="example@domain.com">
                <br><br>

                <label for="password">Password:</label>
                <input type="password" id="password" name="password" required minlength="6" pattern="(?=.*\d)(?=.*[a-zA-Z]).*">
                <br><br>

                <label for="age">Age:</label>
                <input type="number" id="age" name="age" min="18" max="120" required>
                <br><br>

                <input type="submit" value="Register">
            </fieldset>
        </form>
    </section>

    <!-- Table -->
    <section>
        <h2>Schedule</h2>
        <table>
            <tr>
                <th>Day</th>
                <th>Activity</th>
            </tr>
            <tr>
                <td>Monday</td>
                <td>Video Recording</td>
            </tr>
            <tr>
                <td>Tuesday</td>
                <td>Audio Editing</td>
            </tr>
        </table>
    </section>

    <!-- List -->
    <section>
        <h2>Features List</h2>
        <ul>
            <li>Multimedia Support</li>
            <li>User Registration</li>
            <li>Responsive Design</li>
            <li>Interactive Elements</li>
        </ul>
    </section>

    <!-- Footer -->
    <footer>
        <p>Contact: info@example.com | © 2025 Multimedia Webpage</p>
    </footer>
</body>
</html>
