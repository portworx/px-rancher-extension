# px-rancher-extension

Portworx is a software-defined storage overlay that enables high availability for containerized stateful applications across multiple nodes and cloud environments. It allows seamless migration of workflows between clusters, supports hyperconverged workloads by co-locating data and applications, and offers programmatic control over storage resources.

This extension provides monitoring capabilities for Portworx storage in Rancher UI.

## How to add Portworx Extension to your Rancher UI.

In Rancher UI, navigate to Extensions > Manage Repositories > Create
Provide a Name for the repository and select "Git repository containing helm chart or custom template definition"

Provide the following values:

> Git Repo URL: https://github.com/portworx/px-rancher-extension.git

> Git Branch: main

Now click Create.
Now Navigate to Extensions Page and under Available tab, an Extension for Portworx will appear. Install the latest verion.

