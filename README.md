# Placement Maker
This is another script I made at Nativo to perform bulk updates to the database.

This script operates under the assumption that you are given a placement id and then asked to create a new placement for every section in the publication based on that id.

You are also not allowed to use a .csv file and need to solve this problem using only sql and python.

To do this I ended up creating a sql statement that uses the given placement id to determine the publication for that placement and then lists out all the sections that publication has in it. Once that list is available it then iterates over the list and creates a new placement for each section.

So in this case the python function includes a few parameters and then uses the arguments when the function is called to populate the sql queries, but most of the heavy lifting is performed by the sql queries.

This was a bit more of a challenging use case, and I had a lot of fun creating this one.