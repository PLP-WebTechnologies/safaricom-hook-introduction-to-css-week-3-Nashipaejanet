## **🎓 CSS Basics Assignment**  

### **Assignment Title**  
**"Mastering CSS Basics: Styling Your First Web Page"**  

---

### **📋 Objectives**  
- Understand the use of CSS selectors, properties, and values.  
- Apply inline, internal, and external CSS to style web pages.  
- Utilize basic CSS properties to control colors, fonts, alignment, padding, and margins.  

---

### **📂 Assignment Tasks**  

#### **Part 1: CSS Basics - Selectors, Properties, and Values (20 Points)**  
1. Create an HTML file with at least three different types of elements (e.g., `<h1>`, `<p>`, `<div>`).  
2. Style these elements using:  
   - **Element Selector**: Change the font size of all headings.  
   - **Class Selector**: Apply a background color to specific sections.  
   - **ID Selector**: Add a border to an element with a unique ID.  
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Page</title>
    <style>
        /* Element Selector: Change the font size of all headings */
        h1 {
            font-size: 36px;
        }

        /* Class Selector: Apply a background color to sections with class 'section' */
        .section {
            background-color: lightblue;
            padding: 20px;
        }

        /* ID Selector: Add a border to an element with ID 'unique' */
        #unique {
            border: 2px solid red;
            padding: 10px;
        }
    </style>
</head>
<body>
    <h1>Welcome to My Styled Page</h1>
    <div class="section">
        <p>This is a paragraph inside a section with a background color.</p>
    </div>

    <div id="unique">
        <p>This paragraph has a border applied using the ID selector.</p>
    </div>

    <div class="section">
        <p>This is another section with the same background color.</p>
    </div>
</body>
</html>



#### **Part 2: Inline, Internal, and External CSS (30 Points)**  
1. Use **inline CSS** to style one element (e.g., change the text color).  
2. Add **internal CSS** in the `<style>` tag within the `<head>` section to style at least three elements.  
3. Create a separate **external CSS file** and link it to your HTML. Use it to:  
   - Change the background color of the webpage.  
   - Style links with hover effects.  


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Complete CSS Styling Example</title>

    <!-- Internal CSS -->
    <style>
        h1 {
            font-size: 36px;
            color: green;
        }

        p {
            font-family: Arial, sans-serif;
            color: navy;
        }

        .highlight {
            background-color: yellow;
            padding: 10px;
        }
    </style>

    <!-- Link to External CSS -->
    <link rel="stylesheet" href="styles.css">
</head>
<body style="color: purple;">

    <!-- Inline CSS -->
    <h1 style="color: red;">This is a Heading with Inline CSS</h1>

    <p>This is a paragraph with internal CSS applied (font-family and text color).</p>

    <div class="highlight">
        <p>This section has a yellow background color and padding applied via internal CSS.</p>
    </div>

    <a href="https://www.example.com">Visit Example Website</a>
    
</body>
</html>

External CSS file (styles.css)

body {
    background-color: lightgray;
}


a {
    color: blue;
    text-decoration: none;
}

a:hover {
    color: red;
    text-decoration: underline;
}


#### **Part 3: Basic Styling Properties (50 Points)**  
1. Apply the following styles:  
   - **Colors**: Set text and background colors for different elements.  
   - **Font Styles**: Change the font family, size, and weight of text.  
   - **Text Alignment**: Center-align, left-align, or justify text in paragraphs.  
   - **Spacing**: Add padding and margin to elements for proper spacing.  
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Page Example</title>
    <style>
        /* Set text and background colors for different elements */
        body {
            background-color: lightgray;
            color: darkslategray;
        }

        h1 {
            color: darkblue;
            background-color: lightblue;
            padding: 20px;
            text-align: center;
        }

        p {
            color: darkred;
            background-color: lightyellow;
            padding: 10px;
            margin: 10px 0;
        }

        /* Change the font family, size, and weight of text */
        h2 {
            font-family: 'Arial', sans-serif;
            font-size: 28px;
            font-weight: bold;
            text-align: left;
        }

        .footer {
            font-family: 'Courier New', Courier, monospace;
            font-size: 14px;
            font-weight: normal;
            text-align: center;
            margin-top: 30px;
        }

        /* Text Alignment */
        .justify-text {
            text-align: justify;
            margin: 15px;
        }

        .center-text {
            text-align: center;
        }

        .left-text {
            text-align: left;
        }

        /* Spacing: Add padding and margin to elements */
        .spaced-section {
            padding: 20px;
            margin: 20px;
            background-color: lightgreen;
        }

        .spaced-footer {
            padding: 15px;
            margin-top: 30px;
            background-color: lightcoral;
        }
    </style>
</head>
<body>

    <h1>Welcome to My Styled Page</h1>

    <p>This is a paragraph with dark red text and light yellow background.</p>

    <div class="spaced-section">
        <h2 class="center-text">Heading 2 - Centered</h2>
        <p class="justify-text">This paragraph is justified, meaning the text is spread out to align with both the left and right edges of the container.</p>
    </div>

    <div class="spaced-footer">
        <p class="left-text">This footer text is left-aligned, with padding and margin added for spacing.</p>
    </div>

    <div class="footer">
        <p>This is the footer of the page, centered and styled with a different font family.</p>
    </div>

</body>
</html>

2. Create a **simple card component** using these styles:  
   - A heading for the card title.  
   - A paragraph with some description.  
   - Add padding inside the card and a margin around it.  
   - Use a light background color and a subtle border.  

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Card Component</title>
    <style>
        /* Styling for the card */
        .card {
            background-color: #f9f9f9; /* Light background color */
            border: 1px solid #ddd; /* Subtle border */
            border-radius: 8px; /* Rounded corners */
            padding: 20px; /* Padding inside the card */
            margin: 20px; /* Margin around the card */
            width: 250px; /* Set a fixed width for the card */
            box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1); /* Subtle shadow for depth */
        }

        /* Card title styling */
        .card h2 {
            font-size: 24px;
            color: #333; /* Dark text for contrast */
            margin-bottom: 10px; /* Space below the heading */
        }

        /* Card description styling */
        .card p {
            font-size: 16px;
            color: #555; /* Slightly lighter text */
            line-height: 1.5;
        }
    </style>
</head>
<body>

    <!-- Card Component -->
    <div class="card">
        <h2>Card Title</h2>
        <p>This is a simple card component. It contains a heading, a paragraph description, padding inside, and a subtle border for styling.</p>
    </div>

</body>
</html>


This assignment will solidify your CSS basics while giving you a chance to style your first webpage creatively. Good luck and happy styling! 🎨🚀
