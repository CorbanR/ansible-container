Instructure Core
----------------
WIP/POC of using ansible-container to build instructure base images.

see [ansible-container getting started](https://docs.ansible.com/ansible-container/getting_started.html)

run `make` from `instructure/` directory

  Example: `make ruby2.3`



Issues
------
* Unable to specify custom name/tagging of images (it is on the [roadmap](https://docs.ansible.com/ansible-container/roadmaps/roadmap_0_2_0.html))
* container.yml is based on docker-compose v1. Would be better if it was v2.
