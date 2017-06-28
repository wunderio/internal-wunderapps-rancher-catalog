# Athena PDF generation service

https://github.com/arachnys/athenapdf

## Docker

### Compose

We have taken the docker-compose directly from the athena github repo and have rewritten
it only to make it more usable with rancher.

1. converted to version 2 syntax
2. env file is now inline env variables, so that we can convert them into questions
3. renamed service from "static" -> "weaver"

### Images

Currently we just use the docker registry image, which is not verified, not is it even
well documented.  The repo contains a dockerfile which we could use to build our own 
image.
