## Building HTML Based on JSON Data

Using the project starting files, you will be building a web page that displays HTML built from data loaded from a JSON file.

Each time the user clicks the "Load Data" button you will read one item from the JSON data array held in data.js and display that in the main section, inside the div id="output1". If there is already some data in the main section output div then you are to copy that data into the sidebar section's output div BEFORE you insert the new data. The main section will only ever hold one item. The sidebar will be like a history of items viewed.

### Setup

 * If you haven't yet forked the MAD9014 repo, fork it and clone it to your laptop.
 * If you've already forked the repo, do a `git pull` to update your local copy with the latest source.
 * Make sure you have the MidTerm subfolder cloned to your laptop.
 * Download the node.js installer from http://nodejs.org .
 * Install node and npm, and use `npm -g install serve` to install "serve", a tiny webserver (you may need to run `sudo npm -g install serve` if you haven't got root privileges).
 * You can run `serve` on the command line in the folder where your files are.

### Requirements

 * Execute code after the document is loaded using the DOMContentLoaded event listener.
 * When the user clicks on "Load", do an AJAX call to fetch the data
 * When the user clicks on the "Load" button, immediately disable the button by removing the enabled class, adding the disabled class and remove the event listener
 * After the data arrived, enable to "Show first" button by adding the appropriate class and binding the appropriate event
 * When the user Clicks on "Show First", display the first element of the data that was fetched by the server.  The data should include the image, the name formatted with capital letters as the first letter of the first and last name as well as the email address in a <a> tag so that the link is clickable.  That data should appear on the left side.
After the user clicked on "Show first", the text of the button changes to "Show next"
 * When the user clicks on "Show Next", the user that was displayed is move to the right column and the new user is displayed in the left column.
 * There should never be more than 3 users displayed in the right column
 * The right column should display the thumbnail picture and a <a> tag with the email as an href and the name as the text of the link
