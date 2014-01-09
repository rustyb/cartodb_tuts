### Summary
This video tutorial will show you the basics of using filters to explore your data. Filters can be handy when looking for trends and patterns in your data. You can use them to find out how the values in different columns are spread throughout your data. You can also combine multiple filters to really dig deep into what your data contains. Use the filters directly on your maps to see the results or even share maps of filtered results with others.

### Data Sources
Go to your cartodb account and head on up to the common data link and we will import one of our favorite datasets that is the Populated Places dataset from Natural Earth. Click on the Populated Places title and cartodb will begin to import this data into a table on your account.

[Natural Earth Data](http://www.naturalearthdata.com/): data for borders, coastlines, cities, and many other useful collections!

![img1](img/1.png)

### Styling your Data
Once that table has been imported head straight over to the map. You are going to apply some styles so that you can see the view changes made by the filters more easily. When you click the map view tab you will be presented with a map which looks like this:

![img1](img/2.png)

Ok as you can see it’s looking pretty busy! First you should reduce the size of the markers themselves. You can do this by clicking the wizards icon under the  SQL icon. Then you should change the value for the marker size and its stroke to something like the values shown in the images below.

![img1](img/3.png)

It might also be a good idea to change the basemap so that you can also see the markers much more clearly. For this type of work we prefer the CartoDB Dark layer which you can apply by clicking the Basemap dropdown on the top right and selecting the CartoDB Dark Layer.

![img1](img/4.png)

Ok now that we can see our map more clearly lets get adding some filters to the map.

### Adding Filters
Ok so you should now go back to your table view by clicking the table tab on the nav bar at the top.

![img5](img/5.png)

The way you add filters is by using the data that is contained within your columns. So you are going to use a column which is easy to understand and interpret. For instance you could use the pop_max which is the total population for the metropolitan area of each city in the table.

In order to add a filter you click the filter tray icon from the right menu bar below the SQL icon.

![img6](img/6.png)

When you click this you are presented with the view below. You must select the column you wish to filter by from the drop down. In this case you should scroll through the list until you find the pop_max column.

![img7](img/7.png)

CartoDB will then do a quick lookup on your column and create a simple histogram of your column. As you can seen from this distribution there are many areas which have a very low population level on the left while there are very few on the right where the highest values of population are. 

![img8](img/8.png)

So for instance if you wanted to only see those cities with the lowest population levels you will drag the slider so that only the first bar of the distribution is selected as you can see below. As you can see from the numbers above the selection that this has now changed to a value of 0 - 1 million or less.

![img9](img/9.png)

Next you should return to the map to see the results.

![img10](img/10.png)

Cool right? Ok so maybe you couldn’t see those changes too easily. So now you should click the filter icon on the right again while you are still in the map view. Now you have the filter view back up. Drag the selector all the way to the right so that all the cities are selected. The map will automatically update as you change the filter.

Finally you may want to see only those cities which are on the tail of the distribution, the majority of the large cities so to speak. Drag the slider out to select only the smaller bars as shown below.

![img11](img/11.png)

The map is now less clutter with cities as there are far fewer cities of over a million people.

Ok so now maybe you want to add another filter where you will only show capital cities which have a population larger than 1 million people. To do this you should click the plus sign under the distribution for pop_max and then select the column adm0cap.

![img12](img/12.png)

This column is the one which tells you whether the city is a capital city or not. One thing you will notice that the column only has two values 1 or 0 (true or false) hence this interesting looking distribution.

![img13](img/13.png)

So now you should select only those that are capitals, so only those rows where **adm0cap** is equal to **1**.

![img14](img/15.png)

If you no long want a filter it is easy to remove one. In this case you will remove the filter that is only showing the cities of over 1 million people. To do this simply click the small X above the filter as you can see below:

![img16](img/16.png)

If you go back to the table view your filter from the map will be applied here and you can scroll through the table and see what are the names of the cities which are capitals.

![img12](img/17.png)

### Publish your filtered map
Ok so now that you have a map which is showing only the world's capitals and is styled in a way you think looks great. It is very easy to publish a visualization of your map to your friends, colleagues and the world. You should click the visualize button on the top right of the page and then published that visualisation you will no longer have to do any map manipulation for your viewer to see only the map of capitas. 
Click the green Publish button in the top right of the page. From here you can customize how your published map is presented, including zoom and center, which interface elements to display, toggling layers, social media links, etc. At the bottom you will find a URL to share your Visualization via Twitter, email, or anywhere else. When you share that link, viewers will only be able to explore it on the map, they will not be able to edit any of your data.

![img12](img/18.png)


