# Wine Festival Tables

In this project, we’re going to practice tabular organization in HTML so you can hone your skills and feel confident taking them to the real world. Why? If you’re going to have data on a webpage, you’ve got to master the skill of effectively and aesthetically organizing it – an HTML table is the perfect solution.

Wine Festival Schedule
The Aguillar Family is hosting their annual wine festival and they have asked you to build a web page for the event schedule! Use your knowledge of HTML to display a table to the attendees.

You can preview the final version at this link.

Let’s begin!

If you get stuck during this project or would like to see an experienced developer work through it, click “Get Unstuck“ to see a project walkthrough video.

Tasks
10/10 complete
Mark the tasks as complete by checking them off

In index.html, inside of the <div> element that has the attribute class with a value of "container", create a new <table> element.


Inside of the <table> element, add a section for table headings using <thead>.

Then, add two rows inside of it using the table row element.


Inside the first table row element, from task 2, add a table heading element.

Inside of that, include an <h1> with the following text: Wine Festival Schedule.


Inside the second table row element, from task 2, add two <th>s:

In the first, add an <h2> that says Time.

In the second, add an <h2> that says Event.


You may notice that “Wine Festival Schedule” does not stretch across the entire table. Let’s fix that!

In the opening <th> tag of this element, add colspan="2".


Below the closing </thead> tag, section off the table using the table body element.


Inside of the table body you created in the previous task, create 5 rows using the table row element.


Inside each row, create two cells using the table data element.

The first table data in each row should have the attribute class with the value "left".


Inside each of the 5 <td class="left"> elements, add <h3> elements that include the times of the events:

12:00 PM
01:00 PM
02:00 PM
03:00 PM
04:00 PM
Feel free to look back at the live site to compare.


Inside each of the <td> elements that does not have a class attribute with a value of "left", add <h3> elements that include the name of events:

Welcome Reception
Storytelling & Tasting
Wine Luncheon
Aguillar Family Wines
Wine & Cheese Tasting
You have created the events table. Cheers!