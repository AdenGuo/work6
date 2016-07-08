# Summary


Trafficking of children is a very serious problem in China. I collected and organized information in [Baobeihuijia](http://www.baobeihuijia.com/), a famous website for people looking for their lost childern(the name of the website means darling home coming). Through these data and D3.js, I want to tell a sad story about childern who are separated from their families. The visualization can be seen at:
http://bl.ocks.org/AdenGuo/raw/ed01b2d8bed119a88a5b9cd82453196a/


# Design


Main consideration of this data visualization is to use "martini" style. I show readers a story. After the story is shown to readers, more information is left for reader to explore.


The main idea of the story telling part of the data visualization is the intense of childern kidnapping in China. The visualization want to give readers a feeling that so many kids are lost in China. In the interaction part of the visualization, I want to convey the names of every child who can not find their parents. The main point here is this could be a huge list and every name in this list represent the saddest story ever happened to the family. 

I use a rapidly changing circle to represent a kidnapping event. Because I think the changing red circles can indicate alarming incidents. I use brightness of red color to represent the number of missing childern in different provinces. I think that red color can be used to indicate the severity of a fact. I use list of people's names to present the lost of childern is about each family involved. Bacause I believe that names can tie the cold figures to each person and show this tragedy is only about people. I use bar plots to illustrate distributions of missing childern among age, date and gender. Bar plots are suitable for comparing categorical data. 

Initial design is just story telling and names shown based on provinces. However, after several feedback, I think more interative information should add to allow users to explore more truth of the story. Two important histogram of childern is added to the visualization. One is about ages when they lost and the other is about year when they lost.


Several decisions are made according to feedback. First, the hover over province to see the list of names was changed to click to see the list so read can get a close look at the huge list of kids who were missing. The reason I don't use a scroll bar is I want the list look huge to impress readers. Second, some bubbles are out of border of China. The locations of bubbles are randomly generate within certain area(the province). So accidentally, some bubbles are out of border. Third, the title of the visualization is intentionally show on the left upper corner of visualization. I want reader only to focus on one thing in the visualization in one moment. Forth, the reason why trafficking of children is serious in China is well beyond this visualization. So the information of reasons are not shown. Readers can read at:


http://www.ft.com/cms/s/2/9704cbdc-8eaa-11e5-8be4-3506bf20cc2b.html#slide0     


# Feedback


* Karthik Rajasethupathy


Hey Yading, I really like this visualization. it definitely makes an impact and i feel like it tells a story with the way that starts with individual cases and sort of speeds up. some really minor things - when i hover on a province to try to read the names of the kids, if i scroll down, the names disappear. might be nice to make that list more permanent if, for instance, i click a province? also, you start off by showing the ages of the kids, but in the final view, there's no age data. would be informative to break down the number of kids kidnapped in each province by the age group (and show it, possibly as a table or bar chart, in the same area where the count/names are shown?). thanks for sharing, very nice!

My response: changing hover over to click to make the list stay. Adding bar plots for age and lost date.


* Lekhraj Sharma


Hi Yading, really nice visualization. Liked the way you build up visualization by animating bubbles into the map (some bubbles do seem to go out of map in initial animation). Also liked the hovering over info with list of names. Here are few things for you to think about:


-Showing legend for heatmap colors

My response: color are onlyu for comparing, actual number can be obtain by clicking each province.

-Making title of the graph bit bigger and centered

My response: Font of title now is bigger. 

-Currently your name list on hovering can become real long (e.g. 2735 cases in Sichuan) and is hard to read. Consider showing this in a separate scroll-able list view. It may also solve the problem Karthik points out.

My response: Already fix the problem by changing hover over to click. scrollable list is not suitable to represent the length of the list.

-Since you continue to show the last selected region info summary on the right see if you can show the last selection visually in the map as well.

My response: Now the clicked province is high-lighted.

-Might be worth showing a slide bar for year selection to allow user to choose the year range to explore how kidnapping patterns changed across the years.

My response: A yearly distributed plot is added.

-As Karthik suggests, may be good to allow user to slice the kidnapping by age group if possible.

My response: A agely distributed plot is added.

-See if showing percentage of kids (or total kids population in that province) helps to see where are the problem spots.

My response: Text is added to explain the plots.

-Any commentary or insight on why certain regions are worse off (e.g. cities with more crime) may be inetersting read.

My response: Text is added to explain the plots.

-See if you can make visualization responsive. Currently visualization does not scale when browser window is resized.

My response: Fixing it

* Amit Bissa


By showing there names, you have done is captured every individual.....i liked that.


My response: Thank you!

* ucaiado


Wow.... your visualization is shocking (and sad). You have collected a very interesting and important dataset to explore, and I feel like that the way you chose to present the data is just right. Your visualization is beautiful. Congrats !


Related to the technical side, it can be my browser, but some bubbles are showing up out of the map. Is it correct?

My response: It is correct.

As a suggestion would be interesting if you include a bar chart, maybe, with the total number of kids kidnapped by year. You could even use it to allow the user to filter out the data. You know, your message is very clear, and your visualization is great, it is just for curiosity if you are in the mood. 

Uirá

My response: Bar plot and text is added to explain the story.


Iterations:

Three iterations are following(the main index.html can be found in github repo):

The initial version:

http://bl.ocks.org/AdenGuo/raw/05881ceb67dde972a3ef2d1205d3149e/

The version of first submit:

http://bl.ocks.org/AdenGuo/raw/af9a4d5c33fafd47219b22d2f706bc1f/

The version of second submit:

http://bl.ocks.org/AdenGuo/raw/ed01b2d8bed119a88a5b9cd82453196a/

# Resources


http://www.baobeihuijia.com/index.aspx --data source


http://www.ourd3js.com/wordpress/?p=296 --map of China


http://bl.ocks.org/bycoffe/5575904 --point in a shape algorithm


https://bl.ocks.org/mbostock/3048450 --histogram layout


http://guns.periscopic.com/?year=2013 --idea inspiration


http://colorbrewer2.org/ --color use 


http://leafletjs.com/examples/choropleth.html --map interation


http://tributary.io/inlet/5998335 --histogram program


And mighty google.com and stackoverflow.com.