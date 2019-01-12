This project is an attempt to serve a Vue app through Django's Development server. But I am not able to make things work.

I was able to run the vue app on itself, as I am able to run the Django dev server. 
But browsing to the page on http://127.0.0.1:8000/ produces a blank page.

When I use the chrome browser inspection to inspect the html, I can see that the statement:

{% render_bundle ‘app’ %}
is replaced by :
<script type=”text/javascript” src=”http://0.0.0.0:8080/app.js"></script>

However, the inspection shows an error:
Failed to load resource: net::ERR_ADDRESS_INVALID app.js:1

At this point I have no idea how to solve this.