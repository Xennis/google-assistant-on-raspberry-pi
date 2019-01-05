# Ansible Playbook: Google Assistant on a Respberry Pi

[![Build Status](https://travis-ci.org/Xennis/google-assistant-on-raspberry-pi.svg?branch=master)](https://travis-ci.org/Xennis/google-assistant-on-raspberry-pi)

See [
Introduction to the Google Assistant Library](https://developers.google.com/assistant/sdk/guides/library/python/). It explains step by step how to run the Google Assistant on a Respberry Pi.

### Setup Google Cloud Platform project

Enable the required API
```sh
gcloud --project ${GCP_PROJECT} services enable embeddedassistant.googleapis.com
```

### Setup the Raspberry PI

Requirements:
* Ansible is installed
* The [client secret key was created](https://developers.google.com/assistant/sdk/guides/library/python/embed/register-device#download-credentials) and is stored in the home diretory of the pi user

```sh
ansible-playbook google-assistant-on-pi.yml
```
