# Controller Gateway

Configure a Gateway in NGINX Controller with GitHub and Ansible Tower.

Send the vars.yaml to the webhook.  The play will take care of the rest.

When configuring the Template in Tower be sure to have the credential set for the NGINX Controller.

The Model is that this play is maintained alone from the configurations.
One repository per gateway.
 - if the gateway needs to be duplicated per environment, simply change the environment variable.
It is expected that the repo will post to the Ansible webhook on change.
Controller will take care of the rest.

The included vars.yaml is an example.