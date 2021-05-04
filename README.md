# UFOs
## Overview of the analysis:
The purpose of the project was to create a webpage and dynamic table with filters using JavaScript and Bootstrap.
1. Build & format a webpage using bootstrap & css
2. Understand significance of directory structure to organize files being referenced
3. Use javascript to perform the following:
   <br/> -Build & populate a data table
   <br/>-Create an interactive search for user to filter data in the displayed table
   <br/>-Use of If statement to populate filter elements
   <br/>-Use of loop to go through all filter elements & check if they apply to the table
   <br/>-Update the table based on filters applied
## Results
<br/>1. We need to collect inputs from user on what they want to filter. This is achieved through use of D3 SelectAll upon a change event. We use this event to call a function to update our filters.
<br/>![Screen Shot 2021-05-04 at 6 44 41 PM](https://user-images.githubusercontent.com/77771292/117078943-d6cc7800-ad08-11eb-8173-3c654779acc6.png)

<br/>2. Using an empty "dictionary" called Filters, we collect the values input by user to filter and they are organized according to the id for input box they are applied: date, city, state, shape.
<br/>![Screen Shot 2021-05-04 at 6 46 16 PM](https://user-images.githubusercontent.com/77771292/117079056-07acad00-ad09-11eb-8e0d-60baec34581e.png)

<br/>3. Using the now populated Filters dictionary, we need to update our table to only show rows with matching data. For reference, these resources were used: Object.entries reference forEach loop reference
<br/>![Screen Shot 2021-05-04 at 6 48 09 PM](https://user-images.githubusercontent.com/77771292/117079187-4c384880-ad09-11eb-88c8-0d1ad5c33300.png)

## Summary
One drawback of this web page is the cases where no data is found. Empty table is returned, but to be more user friendly there should be some confirmatin message to the user that the filter conditions they have applied do not exist in the data set. Furthermore, the data set is static and limited to a brief period of 2010. To make more useful, I would recommend the following changes:

Collect user input to update the data set with new UFO sightings to expand the data set or connect site via API to a UFO database.
Further refine the filter to return message if no data found.
Make the input boxes reactive so they update table as inputs are entered not requiring a full entry and key to be pressed.
Allow partial or case insensitive search
