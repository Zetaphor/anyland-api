# Anyland API

This is an unofficial effort to document the backend of Anyland.

These endpoints and documentation were generated manually by inspecting network requests via Wireshark as well as exploring the decompiled application source.

Any authenticated requests will require the cookie value to be provided. This cookie value is generated when you hit the `startAuthenticatedSession` endpoint with the `ast` value. Unfortunately the only way I've seen of generating the `ast` value is by launching the client via Steam and logging in, since the `ast` is a session token coming from the Steam SDK. This means the simplest way to grab the session cookie is to inspect network requests post-login and grab it from there.

These requests are all in cURL format, which were manually exported from my Postman collection:

https://www.postman.com/solar-spaceship-436264/workspace/anyland/folder/418303-b480071a-6d95-473b-9684-a3575d44c7dc

I've also included the export Postman collections for convenience.

This also includes a working collection for [Bruno](https://github.com/usebruno/bruno) which is preferred over Postman. The Postman collection will not be updated going forward.

In addition to the cURL requests are saved JSON responses from the server, so we can eventually work on a custom server.