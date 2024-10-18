# Troubleshooting gcloud

### Resetting the default project

If you use gcloud normally to access a different GCP project, you can unset this configuration:
#####
    gcloud config unset project

### Reconfiguring your gcloud after the challenge

- Set your previous default project again:
#####
    gcloud config set project <project>

- Authenticate with your usual account:
#####
    gcloud auth login
#####
    gcloud auth application-default login

### Check which account you are currently using

#####
    gcloud auth list

