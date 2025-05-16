# Deploy an internal developer portal in 15 minutes

This demo shows how to use Red Hat Developer Hub to bootstrap new applications,
and request their deployment using a Git-based workflow.

## Steps

1. Access an instance of Red Hat OpenShift using [Developer Sandbox](https://developers.redhat.com/developer-sandbox).
1. Create a Secret named `github-secrets` in your target namespace using the example _github-secrets.yaml_ in this directory ([this blogpost](https://developers.redhat.com/articles/2025/01/07/backstage-authentication-and-catalog-providers-practical-guide#backstage_authentication_providers) has more details on the secret).
1. Select the **Add** menu from the Developer Perspective and search for the Helm Chart.
1. When deploying the Helm Chart, replace the sample YAML with the _values.yaml_ in this directory.

Ask an attendee for their GitHub handle while waiting for the deployment to complete. Add them to the *evans-developer-demos*
GitHub Organisation. Login to the newly deployed instance of Red Hat Developer Hub, and show that the attendee identity is
synced into the Software Catalog showing that they'll have access too.

Explain that the GitHub integration was setup in our organisation ahead of time,
but it's a standard GitHub Application with permissions assigned.

1. Now, use the **Next.js** template to create an application.
1. After the applicaiton is created show it in the Catalog and in GitHub.
1. Show that Github Actions is being used to build a container image.
1. Show that the new application can be deployed using the **Deploy Application to Environment** template.
1. Open the new deployment Pull Request and explain that only certain team members can merge it.

Explain that once merged the application will be deployed using GitOps.

_NOTE: Make sure to add/update the callback URL for your the GitHub Application being used to authenticate._
