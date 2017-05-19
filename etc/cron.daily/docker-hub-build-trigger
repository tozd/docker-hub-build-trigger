#!/bin/bash -e

. /dev/shm/cron-environment

if [[ -n "$DOCKER_IMAGE" && -n "$TRIGGER_TOKEN" ]]; then
  chpst -u nobody:nogroup /usr/bin/curl --output /dev/null --silent -H "Content-Type: application/json" --data '{"build": true}' -X POST "https://registry.hub.docker.com/u/${DOCKER_IMAGE}/trigger/${TRIGGER_TOKEN}/"
fi
