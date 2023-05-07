# Deadline

Modify this file to satisfy a submission requirement related to the project
deadline. Please keep this file organized using Markdown. If you click on
this file in your GitHub repository website, then you will see that the
Markdown is transformed into nice looking HTML.

## Part 1: App Description

> Please provide a firendly description of your app, including the
> the primary functions available to users of the app. Be sure to
> describe exactly what APIs you are using and how they are connected
> in a meaningful way.

> **Also, include the GitHub `https` URL to your repository.**

The app is designed to accept the title of a book as its input, and returns a list of media
associated with the book's author. For example, searching up 'Harry Potter' returns different
movie, video game and other adaptations of J.K. Rowling's works.

The user input is passed into an OpenLibrary API, which pulls the name of the author.
This name is then passed into one IMDb API, which pulls the ID of the author only if their names match exactly
in both APIs (Note that exceptions may occur in the case of authors that share a full name with others in the IMDb database.
This ID is then passed into yet another IMDb API, and then returns a list of titles, years and (in some cases) images of
said adaptations. The reason I used two different IMDb APIs is that it ensures that I am filtering through the results correctly.
For example, the second API helps ensure that J.K. Rowling is listed as a "Writer" for the adaptations.

Git URL: https://github.com/AkilMirUGA/cs1302-api.git

## Part 2: New

> What is something new and/or exciting that you learned from working
> on this project?

One thing I found really exciting to learn from this project was how different companies have different ways to access APIs.
Some give it away for free, whereas some require an API key, and some involve even tighter restrictions.



## Part 3: Retrospect

> If you could start the project over from scratch, what do
> you think might do differently and why?

One thing I might do differently is implement my scene graph first. My approach for this project was to ensure the jsons were parsing correctly
first, but this made testing a little more complicated and hard to read than it wouldve implementing the graph first.
