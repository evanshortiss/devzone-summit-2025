# Deploy an internal developer portal in 15 minutes

This demo demonstrates how Red Hat Developer Hub's Helm Chart simplifies deployment of Backstage on Kubernetes/OpenShift.

## Steps

1. Access an instance of Red Hat OpenShift using [Developer Sandbox](https://developers.redhat.com/developer-sandbox).
1. Create a Secret named `github-secrets` in your target namespace using the example _github-secrets.yaml_ in this directory ([this blogpost](https://developers.redhat.com/articles/2025/01/07/backstage-authentication-and-catalog-providers-practical-guide#backstage_authentication_providers) has more details on the secret).
1. Select the **Add** menu from the Developer Perspective and search for the Helm Chart.
1. When deploying the Helm Chart, replace the sample YAML with the _values.yaml_ in this directory.

Ask an attendee for their GitHub handle while waiting for the deployment to complete. Add them to the *evans-developer-demos*
GitHub Organisation. Login to the newly deployed instance of Red Hat Developer Hub, and show that the attendee identity is
synced into the Software Catalog showing that they'll have access too.

_NOTE: Make sure to add/update the callback URL for your the GitHub Application being used to authenticate_
