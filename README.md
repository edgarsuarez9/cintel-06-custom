# cintel-06-custom

Task 3.  Read About reactive.file_reader
Read about reactive.file_reader by clicking the link above.  This seems very helpful for continuous updates. A reactive.file_reader makes it easy to write apps that automatically update all of their outputs as soon as files on disk change.

Imagine score files getting updated after a game, sales files getting updated each night, web site analytics log files updating every day, and how helpful it could be to read and ingest that data, automatically updating the morning dashboard to show the most recent information. Now try to read the API and the example and see how you might answer these questions. 

What does reactive.file_reader() create?
Is reactive.file_reader() a decorator or a function?
Will reactive.file_reader() watch a whole directory? Or just a single file?
What is the first argument we must provide to the reactive.file_reader() decorator? 
In the example, we apply this decorator to a function named read_file().  How many arguments must this function read_file() function take?
Were you able to answer these questions from the documentation? Share your thoughts or challenges in the discussion. Talking about new features with others is a great way to become more familiar. 

Being able to explain your process in an interview is helpful too - try to verbalize what we're doing so you're comfortable explaining it to others.

Task 4. Plan Your App - Inputs
Our continuous information includes temperatures for multiple locations and stock prices for multiple companies. We might not want ALL information showing ALL of the time. Let's let the user decide what's most important - in this case:

Choose a single location to focus on from the list of possibilities
Choose a single company to focus on from the list of possibilities
Consider all of the ui input options listed in the Shiny Function Reference sidebar menu.Links to an external site.

What is the typical widget for "select one from a list"? 

What would you choose if you wanted to let the user "show or hide" each option individually (hint: checking a box)?

 

Task 5. Plan Your App - Outputs
It can be helpful to start with text, then a table, and ultimately a chart.  

First, just display an output text that confirms to the user input selection. This can be helpful for debugging the reactivity by making sure we have a valid input to react to.
Second, display an output table with the values we need. This allows us to inspect the data and notice how things are changing. 
Third, display an output plot to show things graphically - or use a more advanced widget like we did to use Plotly Express interactive charts. 
When selecting outputs, again refer to the basic outputs listed in the Shiny Function Reference sidebar menu.Links to an external site.

We also used more advanced charts like Plotly Express. For that, we need to use ipywidgets via the shinywidgets package as we did before.  Consider the various charting options: Plotly Express, Altair, Bokeh. Do a quick search and / or ask an AI assistant which are good to learn for your specific use case. Links to an external site.

Task 6. Choose your Data Set - https://pypi.org/project/nfl-data-py/
Choose your data set from the earlier options. Pick one to use for this week's app.

Task 7. Sketch Your Custom App
Choose one of the standard datasets - we asked for your preference earlier, and it may change. Could be a Seaborn data set, or from some other source. For best results, make sure the data is pretty clean. Real-world, messy data is hard to work with. Choose a clean data set and keep the focus on building interactive apps and/or apps for data in motion. Assume you'll load your data into a Pandas dataframe for processing (and maybe a deque if using/simulating live data). 

By sketch, we mean plan your app.py using comments. Clearly indicate where each part of your app will go. Use your earlier examples as guides. Begin adding comments and standard features to your app.py file. 

Imports

Reactive Aspects 

Define at least one reactive calc that can be called by your UI output components
UI Page Inputs

UI Sidebar Components

Choose at least one input that the user can interact with to filter the data set
UI Main Content

Everything not in the sidebar is the main content.
Will you use a template?
Will you use layout columns?
Will you use navigation or accordion components?
Define some output text. Will it be in a card? A value box? 
Define an output table or grid to show your filtered data set
Define an  output widget or chart (e.g., a Plotly Express chart) to show the filtered data graphically
