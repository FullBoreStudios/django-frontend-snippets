# django-frontend-snippets
Helpful snippets of code for doing things with Django and Front End Design


## Bootstrap Carousel
- Link to [Gist Snippet](https://gist.github.com/benmcnelly/8c07d4f965d707b9081311b407678825)

Bootstrap Carousels can be tricky to implement, so here is an example with a few cool things added you can take and leave as you desire.
For one, if you want to use the indicators (little lines at the bottom of the slide) you need to loop over those, and they expect you to provide a data-slide-to="0" element, sequentially numbered starting with 0 (thanks javascript). 

You also need to check if its the first item in the forloop and mark it with an active class. Only one item can start with the active class and only one item can have it at a time. Once the page is loaded the bootstrap javascript will take over assigning the active class. The core concept here is the [forloop](https://docs.djangoproject.com/en/2.1/ref/templates/builtins/#for).

We also wanted to check if there is a link if it was going outside the site to open it in a new window, this of course is set up to use the models we have but if you can take anything from it, enjoy!
