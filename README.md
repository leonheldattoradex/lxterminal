This is a very small example of how to launch lxterminal inside Weston within the TorizonCore operating system.

Simply copy the `docker-compose.yml` file to the target device or use the TorizonPlatform update service to create
a package and either `docker-compose up` (in case you copied the file manually) or wait a bit (in the case of a TorizonPlatform
remote update).

This example is specially target at launching "terminal GUI" applications, in this case we use lxterminal. If that's what you want,
add `--command` according to the lxterminal documentation and it will launch your application inside the lxterminal within the 
Weston compositor.

Naturally, your application has to be available within the container that also has `lxterminal`, so edit `Dockerfile` first.

Note: this is not maintained officialy by Toradex in any way, shape or form.
