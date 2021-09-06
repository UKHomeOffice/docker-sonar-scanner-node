# docker-sonar-scanner-node

**This repo has been deprecated in favour of the [docker-sonar-scanner repo](https://github.com/UKHomeOffice/docker-sonar-scanner). If you require any extras packages, Feel free to fork the repo**

Enables integration with SonarQube including node.js packages required for Typescript code reviews.

### Usage

Insert the snippet below after your build step in your .drone.yml, copy the sonar-project.properties to your project and fill out the missing bits.

```
  sonar-scanner:
    image: quay.io/ukhomeofficedigital/sonar-scanner-node:latest
    when:
      event:
        - push
        - pull_request
```
