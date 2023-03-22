# github-oauth-apps

This repo is just a README.md to document how to create GitHub OAuth apps for the deployment of the GlueOps Platform. 

## Before you start:

For this example we will assume your GitHub organization is called `glueops-rocks`. You will need to update the URL's/links below accordingly to use your organization name in place of `glueops-rocks`. Secondly, we will assume your `captain_domain` is `nonprod.antoniostacos.glueopshosted.com`

### Create the ArgoCD Application

1. Go to: https://github.com/organizations/glueops-rocks/settings/applications

2. Click on `New OAuth App`
3. Let's create an the first app.

- `Application name`: GlueOps-ArgoCD

- `Homepage URL`: https://argocd.nonprod.antoniostacos.glueopshosted.com

- `Authorization callback URL`: https://argocd.nonprod.antoniostacos.glueopshosted.com/api/dex/callback

4. Save the Client ID and Client Secret

### Create the Grafana Application

1. Go to: https://github.com/organizations/glueops-rocks/settings/applications

2. Click on `New OAuth App`

3. Let's create an the first app.

- `Application name`: GlueOps-Grafana

- `Homepage URL`: https://grafana.nonprod.antoniostacos.glueopshosted.com/login

- `Authorization callback URL`: https://argocd.nonprod.antoniostacos.glueopshosted.com/login/github

4. Save the Client ID and Client Secret
