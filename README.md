# raspberry-pi-smart-speaker

[![Build Status](https://travis-ci.org/Xennis/raspberry-pi-smart-speaker.svg?branch=master)](https://travis-ci.org/Xennis/raspberry-pi-smart-speaker)

See [
Introduction to the Google Assistant Library](https://developers.google.com/assistant/sdk/guides/library/python/)

### Setup Google xxx

Enable the required API
```sh
gcloud --project ${GCP_PROJECT} services enable embeddedassistant.googleapis.com
```

### Setup the Raspberry PI

Requirements:
* Ansible is installed
* The [client secret key was created](https://developers.google.com/assistant/sdk/guides/library/python/embed/register-device#download-credentials) and is stored in the home diretory of the pi user

```sh
ansible-playbook pi-smart-speaker.yml
```
