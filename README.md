https://ankitpal7066.github.io/03githubFinder/     


Event Listeners: The code starts by selecting various elements from the DOM using document.querySelector() and assigns them to variables:

searchForm: Represents the form element with the class search-form.
userCardContainer: Represents the element with the class user-card.
loader: Represents the element with the class loader.


getUser Function: This is an asynchronous function that is called when the user submits the form. Here's what it does:

It retrieves the value entered by the user in the keyword input field.
If the input is empty, it displays a loading spinner in the userCardContainer.
If there is a keyword, it fetches data from the GitHub API for the user with the provided username.
It updates the userCardContainer with user information if found, or displays an error message if the user is not found.
Finally, it clears the input field by setting its value to an empty string.


showUser Function: This function takes the user data as an argument and dynamically generates HTML content to display the user's information in a card format. It checks if the user exists by looking at the message property in the API response. If the user is found, it creates HTML elements to display the user's data.

Event Listeners: The code adds event listeners to the form and the theme select element. When the form is submitted, the getUser function is called, which fetches the GitHub user data and updates the page. When the theme is changed, the themeChange function is called to switch between light and dark themes by changing the background and text colors of the body element.
