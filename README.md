# Grove Data Engineering - Neo Challenge

For this challenge you will create an ETL to capture information about NEOs (Near Earth Objects) and produce a visualization from the results.

## Part 1 - ETL

Using any language and database system you are comfortable with, create an ETL to process data from NASA's Near Earth Object Web Service. Your goal is to determine if and when any hazardous objects will be approaching earth, how close they will get, and save the information to a database for review in Part 2.

NASA's web service, including example API calls, can be found here:
https://api.nasa.gov/

Note the NASA API severely rate limits their default public key. It's not strictly required for this exercise, but you can quickly register to get a more expansive API key [here](https://api.nasa.gov/). Please do not include your API key in your submission. 

The ETL should perform the following when invoked:

* Query the API for new data, based on the last record of capture. If there are no records in the database, backfill from a user provided date.
* Capture relevant information about potentially hazardous NEO's for part 2, including the close approach date and miss distance. The boolean field is_potentially_hazardous_asteroid will indicate if an object is potentially hazardous.

## Part 2 - Visualization

Next, create a visualization of near-misses.  Query the database of potentially hazardous objects from task 1 and create a visualization that clearly shows the objects over time and how close they came to hitting the earth.

You can use any graph or charting mechanism you prefer. Please include a screenshot, along with any source if possible. We should be able to easily review your work.

## Submission Guidelines

* Please create a new GitHub repo for your work. Do not fork this one.

* Check all of your source code into GitHub, including any screenshots from Task 2. Please also check in any schema or database exports and/or related database files that you created in task 1 along with instructions. We should be able to get your solution up and running quickly on a mac or Ubuntu Linux system.

Keep in mind we're looking for the following:

* Quality. Is your coding style consistant, clear, and understandable? If hired, is this the level of code you would create to run on our production systems?
* Test coverage.  Do you make good use of testing?  Are there appropriate, well-written unit and/or integration tests? As this is an exercise we don't need complete coverage, but we do want to see how you approach tests and your ability to write testable, maintainable code.

Thanks, and good luck!
