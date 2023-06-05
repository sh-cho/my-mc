## provisioning

### environment

- papermc docker image: https://hub.docker.com/r/marctv/minecraft-papermc-server
- GCP app engine
- (TODO) terraform

### How to deploy

> **Note**
>
> CWD: `/app`

```bash
gcloud auth login
gcloud config set project $PROJECT_ID
```
login and select project

```bash
gcloud projects list
```
(list projects)

```bash
gcloud app deploy
```
Deploy

#### Test locally

TBD

### Reference

- App engine docs: https://cloud.google.com/appengine/docs/flexible
  - testing and deploying: https://cloud.google.com/appengine/docs/flexible/testing-and-deploying-your-app?tab=custom#top
- `gcloud app deploy` docs: https://cloud.google.com/sdk/gcloud/reference/app/deploy
