# Credential Helper
Authorisation for ICCR without `ibmcloud cr login` or `docker login`, see [credential helpers](https://docs.docker.com/engine/reference/commandline/login/#credential-helpers)
 
Requirements:
1. Have a linux like environment with `/bin/bash`.
1. Have the [ibmcloud CLI](https://cloud.ibm.com/docs/cli?topic=cloud-cli-install-ibmcloud-cli) installed.
1. Be logged in.

## INSTALL 
1. place docker-credential-icr-helper in your path
1. add or merge a `credHelpers` object to to your ~/.docker/config.json like this:
```json
 "credHelpers" : {
    "icr.io" : "icr-helper",
    "uk.icr.io" : "icr-helper",
    "us.icr.io" : "icr-helper",
    "de.icr.io" : "icr-helper",
    "au.icr.io" : "icr-helper",
    "jp.icr.io" : "icr-helper",
  },
```
