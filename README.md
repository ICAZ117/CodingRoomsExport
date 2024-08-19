This is a simple export tool for coding rooms problems. Simply paste your coding rooms bearer token into index.html, open the file in your browser, and enter the relevant info:

* Token: Your Coding Rooms auth bearer token - can be obtained from the headers of any request made by Coding Rooms to their API
* Course number: The reference number for the course in CodingRooms' DB - open the network tab of your browser inspector on their page and look at the API request that returns the nativeAssignments JSON object. The request URL contains the numerical course number
* Starting idx: The index which of the problem list from which you wish to begin pulling data. This is 0-based, and the list is sorted alphabetically based on problem name.
* Lang: The filename extension for any code files that need to be save (java, py, cpp, etc.)

Be advised that this code is intended for a server environment; if you run it locally on a browser, you will likely run into CORS issues. This can be resolved by simply using a CORS preflight extension in your browser.
