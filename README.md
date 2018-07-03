# docker-sonar-scanner-node
Enables integration with SonarQube and includes node.js packages required for the SonarTS plugin.	

### Usage

Insert the snippet below after your build step in your .drone.yml, and copy the sonar-project.properties to your project and fill out the missing bits.

```
  sonar-scanner:
    image: quay.io/ukhomeofficedigital/sonar-scanner-node:latest
    when:
      event:
        - push
        - pull_request
```
