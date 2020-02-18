# jenkins-k8s-test
This is a simple repository used for jenkins (running on docker or k8s) pipeline testing.
It contains a php-app for watermarking gallery.
Dockerfile contains all the instructions to build the image.
When running the pipeline first delete the index.html from the repo and its corresponding COPY index.html from the Dockerfile in this repo
Build the image
And then rerun the pipeline placing index.html in the repo
and adding the COPY index.html /var/www/html command in the Dockerfile

