Project - Data Visualization with Titanic Data Set


Summary:

Titanic data set is a very well-defined and popular dataset suitable as a test vehicle for a new project. The story is touching and as a post-mortem vehicle I wanted to explore the survivability of the passengers with respect to several factors that came alongwith this dataset. A curious viewer can interact with the visualization and explore various aspects linked to the survivability of the passengers. Finally, the Summary plot brings about a clear finding that that the female passengers had better chance of survival over men and passengers of higher cabin classes had better luck over the others.


Design:

I focussed on the survivability as the main theme. There are variables like gender, cabin class, port of embarkation etc. that are present in the database. I wanted to give the viewer the ability to disect the survivability data based on these variables. 

I mainly limited myself to creating bar charts. Based on the feedback I have received, I have stayed away from drawing pie chart and unnecessary animation. I would have considered animation if there had been a time series in the dataset.

Color has been chosen as the primary form of visual encoding. Soft and neutral colors have been used as much as possible. Dimple.js had worked great to create the first level plots and some D3 was very helpful to customize various aspects. Based on the feedback, I felt it necessary to design customized tool tips in place of the default ones.

I would have loved to use the 'age' as a variable and plot against it, but realized that a lot of passengers do not have the age information. Besides, I thought I would take more time to learn how to plot histogram like visualization using Dimple.js.


Feedback:

Initial version: index_1.html
       
Three persons have reviewed my first visualization based on 'index_1.html'. Following are their feedback: 

1. Ganapthy Parthasarathy (Colleague - DevOps, Machine Learning expert)

The visualization for the Titanic data should better focus on the survivability. Any person aware of the incident would be curious to know about how many people survived and any correlation that can be drawn to the associated variables.

Initially, I had drawn a pie chart segmented for various ports of embarkation. This was then animated to display gender-wise pies. According to him this animation was not necessary since the same information can be displayed, without distracting the attention, with static plots.

He had general feedback about color and the tool tips. The default tool tips could be replaced by more crisp texts.

2. Ram Ramaswamy (Colleague - EDA tool user interface designer, useability expert)

 A blank canvas, to start with, does not look good. Have a 'default' display.

Animation in the pie chart is unnecessary. Suggested to plot stacked donut charts with increasing radius. Every donut could represent a variable. User can interact with any segment and find survival data through tooltips. I decided to not plot it that way since I thought that the plots would look very busy.

Recommended to implement customized tool tips and neutral colors. The background color of the svg element is very prominent and it is distracting. Make it a lighter color.

3. Avik Das (Son - JavaScript and VR expert)

The vertical axis on the 'Gender' plot is labeled 'Survived'. This is misleading because its really the count of the passengers who may or may not have survived.
             

Agreed with the others that animation does not add much of value for this dataset.

Suggest to flip the x and y axis for the plot with port of embarkation data. i.e. plot the port of embarkation on the x-axis and the survival information along the y-axis. According to him, plotting the bars with port as independent variable helps add more information to the viewer.

The colors of the two bar graphs are flipped This makes it hard to switch between the two graphs because mentally, I am thinking of the colors in the wrong way after switching.
            

Resources:

1. https://d3js.org/

2. http://dimplejs.org/

3. Udacity discussion forum

4. Various blogs of Mike Bostock, incuding:
       https://bl.ocks.org/mbostock/3885304

5. Enter, Update, Exit:  
       https://medium.com/@c_behrens/enter-update-exit-6cafc6014c36

6. Pretty charts with dimple.js: 
       http://annapawlicka.com/pretty-charts-with-dimple-js/

7. Storytelling with data: exploratory vs. explanatory analysis: http://www.storytellingwithdata.com/blog/2014/04/exploratory-vs-explanatory-analysis
