Image daily triggers a Docker image rebuild on Docker Hub.

It is configured through environment variables:
 * `DOCKER_IMAGE` – name of the image to rebuild
 * `TRIGGER_TOKEN` – a token which you can obtain on *Build Settings* page on Docker Hub
   of your Docker image; at the end there is a section named *Build Triggers* where
   you have to first activate triggers
