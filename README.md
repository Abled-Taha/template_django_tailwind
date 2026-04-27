
1. Run setup.sh or setup.ps1 and follow instructions. (MISE must be installed)

NOTE: This template not only contains Django, as well as Tailwind (Standalone) but also contains HTMX, AlpineJS and Animate.css. Along with some other useful features like an empty modal shell to use for anything, robots.txt, django form messages, base.html, home.html, 404.html.

NOTE: Currently all the requests to / are redirected to /web. This behaviour can be changed by changing the main.views.redirect_to_web function, and making any necessary changes in main.urls

NOTE: This is just a template and the names and description are set to be generic, and the ones which could be left empty are empty. The pyproject.toml has been left empty for the name and description. And the django project name is set to be "main" with the "web" app, although it can be removed easily. The libraries are also kept to be very generic or required by this setup.

NOTE: The favicon should also be changed as I just used anything I could find. The favicon is located in /static/img/favicon.png

STEPS TO REMOVE "web" APP:
1. Remove the /web from main.urls and change the / to do something else than to redirect to /web.
2. Remove the importing of "redirect_to_web" function in main.urls and remove the main.views.redirect_to_web function.
3. Remove the "web" entry in main.settings.INSTALLED_APPS
4. Remove the "web" directory.