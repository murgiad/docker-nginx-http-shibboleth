Package build
=============

$ docker run -it --rm -v /var/tmp/debs:/opt/rebuildnginx/debs:rw criluc/docker-nginx-builder:jessie

The you can find the .deb files in your /var/tmp/debs dir.

How to update nginx e nginx-http-shibboleth module
--------------------------------------------------

From this dir (where the Dockerfile is placed)

$ docker build -t criluc/docker-nginx-builder:jessie .

then build the packages again as above:

$ docker run -it --rm -v /var/tmp/debs:/opt/rebuildnginx/debs:rw criluc/docker-nginx-builder:jessie

