# How is this project structure different than a Flask (or Node) application?
- Django has specific ways to do things such as declaring your urls/routes. You create these
in a specific way otherwise it wont work. While something like Flask or Node you mostly have more freedom
to structure your project however you want. 

# What role are the urls.py and views.py files responsible for?
- Urls is where you declare the routes(aka urls) which is where the user will go to view content.
Views are used to do things like fetch things from the database, return HTML and a lot more.
You can think of these as the "face" of the web since it's mostly responsible for showing the content
at the specified route.

# Why do we use 2 separate urls.py files? How do they interact?
- Have different url files depending on the project/app helps keep things organized.
This allows a developer to quickly identify what routes the app within the project is responsible for.
They interact by using something called "include" which is like a pointer to a specific route
which has it's own url rules and handles their own thing.

# When is it desirable to split our code over multiple apps? Why would we want to do so?
- Typically you would want to split the code up depending on the feature you're working on.
Each feature can be it's own app. This promotes an organized structure and makes it easy to
add onto the project and help debug specific features.

