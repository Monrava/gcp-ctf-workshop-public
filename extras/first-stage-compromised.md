# First stage compromise

You extracted a new access token! Let's see what this one can do.  
You can use the tokeninfo endpoint again to find out:  
#####
    curl -i https://www.googleapis.com/oauth2/v3/tokeninfo\?access_token=<token>
Cloud functions by default are also using the compute engine default service account - but with the full `cloud-platform` access scope!  

That should get you a set of nice new permissions on this GCP project.  
You can tell gcloud to use your new token by setting it as environment variable:  
#####
     export CLOUDSDK_AUTH_ACCESS_TOKEN=<function token>

Now, let's try to list the IAM policy on this GCP project to see which project-level access your account has:  
#####
    gcloud projects get-iam-policy $PROJECT_ID

You are Editor on this project which allows you read and write access to almost all resources.  
Congratulations! You compromised this GCP project.  
