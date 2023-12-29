 ## This quote generator app is a simple web application designed to display and share random quotes. Here's a breakdown of its main components and functionalities:



The JavaScript code interacts with the HTML elements using the getElementById method to get references to different parts of the app.

### Loading Functions:

The loading function is responsible for showing a loading state by hiding the quote container and displaying the loader.
The complete function does the opposite, hiding the loader and displaying the quote container when the loading is complete.


### Quote Handling:

The newQuote function is triggered when the user clicks the "New Quote" button.
Inside this function, there's logic to fetch a random quote from an API. The quotes are stored in an array (apiQuotes), and a random quote is selected for display.
If the author of the quote is not provided (undefined), it sets the author text to "Unknown."
The function also checks the length of the quote text and applies a CSS class (long-quote) for styling purposes if the quote is long.


### Fetching Quotes:

The getQuotes function is an asynchronous function responsible for fetching quotes from a specified API (https://jacintodesign.github.io/quotes-api/data/quotes.json).
It uses the fetch API to make an HTTP request and then converts the response to JSON.
Once the quotes are fetched, the newQuote function is called to display a random quote.


### Tweeting a Quote:

The tweetQuote function is triggered when the user clicks the "Twitter" button.
It constructs a Twitter URL with the current quote text and author and opens a new browser window or tab to allow the user to tweet the quote.


### Event Listeners:

Event listeners are set up for the "New Quote" button (newQuoteBtn) and the "Twitter" button (twitterBtn), so that when these buttons are clicked, the corresponding functions (newQuote and tweetQuote) are executed.

### On Load:

The getQuotes function is called when the page loads to fetch an initial set of quotes and display a random quote.
In summary, this app provides a user-friendly interface for generating and sharing random quotes, with an emphasis on a clean design and a seamless user experience.


![2023-12-29_22-51.png](..%2F2023-12-29_22-51.png)

![2023-12-29_22-52.png](..%2F2023-12-29_22-52.png)