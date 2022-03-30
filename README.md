# Quick Setup Guide

This code sets up kibana and elastic in a secure way.

- Point a kibana and elastic domain at your new ec2 instance.
- Clean Ubuntu 20.04 Box (aws).
- Run ./install-docker.sh
- Copy .env.example to .env
- Open up the .env file:
  - set elastic username and password
  - set elastic and kibana urls
  - set memory limits for elastic to use
  - optional: set where you want elastic data to reside on the host system
- Run `sudo chown ubuntu:ubuntu` on entire cloned folder (or user 1000)
- Ensure your elastic data belongs to ubuntu:ubuntu (or user 1000)
- Run docker-compose up -d
- Test your URLs
- Enjoy

