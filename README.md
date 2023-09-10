# Github_Search-
# Hosted Link:-https://tulasidurga1.github.io/Github_Search-/
# explanation :-
The provided HTML code represents a webpage for a "Github Finder Project." Let's break down the code and the accompanying JavaScript and CSS styles:

### HTML Structure:
````` <!DOCTYPE html>: This declaration specifies that the document is an HTML5 document.

1. <html lang="en">: The opening tag for the HTML document, with the specified language attribute set to "en" (English).

2. <head>: This section contains metadata about the web page, including character encoding, viewport settings, and links to external resources.

3. <meta charset="UTF-8">: Specifies the character encoding of the document as UTF-8.

4. <meta name="viewport" content="width=device-width, initial-scale=1.0">: Sets the viewport properties for responsive design.

5. <title>Github Finder Project</title>: Defines the title of the web page, which is displayed in the browser's title bar or tab.

6. <link rel="stylesheet" href="./css/main.css">: Links an external CSS file named "main.css" to style the webpage.

7. <link href="https://fonts.googleapis.com/css?family=Roboto+Mono:100,200,300,regular,500,600,700,100italic,200italic,300italic,italic,500italic,600italic,700italic" rel="stylesheet" />: Imports the Google Fonts "Roboto Mono" font family for use in styling.

8. <link href="https://cdn.jsdelivr.net/gh/hung1001/font-awesome-pro@4cac1a6/css/all.css" rel="stylesheet" type="text/css" />: Includes the Font Awesome Pro icon library via a CDN for using icons in the page.

9. <link rel="stylesheet" href="style.css">: Links another external CSS file named "style.css."

10. <body>: The main content of the web page is contained within this section.

11. Inside the <body>, there's a <div class="container"> that wraps the entire content of the page.

12. <header class="header d-flex between center">: This is the header section of the page, containing a logo with the text "Github."

13. <form class="search-form d-flex between center">: A search form with an input field for entering a GitHub username and a search button.

14. Inside the form, there's an icon (<i class="far fa-fw fa-search"></i>) for search, an input field (<input type="text" placeholder="Search Github username" class="keyword">), and a submit button (<button class="btn" type="submit">Search</button>).

15. <div class="user-card">: Initially, this div contains a loader message. It will later display user information fetched from GitHub.

16. <script src="index.js"></script>: This script tag links an external JavaScript file named "index.js." This JavaScript file contains code to handle user input and fetch GitHub user data.

- JavaScript (index.js):
This JavaScript code is responsible for handling user input, fetching data from the GitHub API, and displaying user information.

Event listeners are set up to listen for the form submission. When the form is submitted, it triggers the getuser() function.

The getuser() function checks if the input field is empty. If it is, it displays a loader message. If not, it sends a request to the GitHub API to fetch user data based on the entered GitHub username.

Once the data is fetched, it's checked for errors (e.g., "Not Found"). If there are no errors, the showuser() function is called to display the user's information in the "user-card" div.

- CSS (style.css):
The CSS code defines styles for various elements on the webpage, including fonts, colors, layout, and positioning. It styles elements such as the header, search form, user card, and various text and icon elements.

It's important to note that this code assumes the existence of specific CSS classes and HTML structure in your "main.css" and "style.css" files, which are linked in the HTML <head>. The styles specified in those files will determine the visual appearance of the webpage.
