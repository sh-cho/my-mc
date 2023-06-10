## provisioning

WIP

### environment

- GCP VM (x86_64)
  - Rocky linux 8.7
- OCI VM (arm64)
  - Rocky linux 9.1
- PaperMC
- Ansible
- (TODO) packer
- (TODO) terraform

#### Pre-requisites

```bash
brew install pyenv
pyenv install 3.10.7
pyenv local 3.10.7
pip install ansible ansible-lint
```
Setup ansible

### Instruction

> **Note**
>
> CWD: `/provisioning/ansible`

#### Setup server

```bash
ansible-playbook -i inventory.ini setup.yml
```

#### Deploy app

TBD

#### Test locally

TBD

### Reference

- App engine docs: https://cloud.google.com/appengine/docs/flexible
  - testing and deploying: https://cloud.google.com/appengine/docs/flexible/testing-and-deploying-your-app?tab=custom#top
  - app.yaml: https://cloud.google.com/appengine/docs/flexible/reference/app-yaml?tab=custom
- `gcloud app deploy` docs: https://cloud.google.com/sdk/gcloud/reference/app/deploy
