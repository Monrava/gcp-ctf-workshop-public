# Using kubectl for challenge 1

1. Create a config file and add the cluster IP and your token:

#####
    apiVersion: v1
    clusters:
    - cluster:
        server: https://<cluster IP>
        insecure-skip-tls-verify: true
      name: ctf-cluster
    contexts:
    - context:
        cluster: ctf-cluster
        user: ctf-service-account
      name: ctf-context
    current-context: ctf-context
    users:
    - name: ctf-service-account
      user:
        token: <your token>

2. Tell kubectl to use this configuration

#####
    export KUBECONFIG=<path to config file>

