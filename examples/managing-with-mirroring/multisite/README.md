# Multisite
This reposiory contains informartion for installing and configuring multisite connectivity.

# Deploying OCP
At least two OCP clusters are required. [ Follow the steps here ](./installation/README.md)

# Deploy ArgoCD
Deploy ArgoCD to each cluster and set the Argo CD password to something meaningful. [ Follow the steps here ](./argo-installation/README.md)

# Setup storage
To setup storage [ Follow the steps here ](./storage/README.md)

# Deploy the wordpress application
Verify the storageclass that you are wanting to use matches what is defined in 

* https://github.com/yard-turkey/examples/managing-with-mirroring/multisite-application/blob/master/wordpress/base/mysql-pvc.yaml
* https://github.com/yard-turkey/examples/managing-with-mirroring/multisite-application/blob/master/wordpress/base/wordpress-pvc.yaml. 

Once the correct values of the storage class has been created [ Follow the steps here ](./argo-apps/README.md) to deploy applications within Argo CD

# Configure cloudflare
Login to cloudflare and [ follow the directions here ](./load-balancing/README.md)

# Mirroring
To begin the process of mirroring the data [ Follow the steps here ](./mirroring/README.md)

# Switching sites
Perform the following steps to switch from site 1 to site 2. [ site 1 to site 2](./failover/README.md)
