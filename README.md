# px-rancher-extension

Portworx is a software-defined storage solution that enables high availability for containerized stateful applications across multiple nodes and cloud environments. It allows seamless migration of workloads between clusters, supports hyperconverged deployments by co-locating data and applications, and provides programmatic control over storage resources.

This extension integrates Portworx storage monitoring directly within the Rancher UI.

## Adding the Portworx Extension to Your Rancher UI

1. In the Rancher UI, go to **Extensions > Manage Repositories > Create**.
2. Provide a name for the repository and select **Git repository containing helm chart or custom template definition**.
3. Enter the following details:
   - **Git Repo URL**: `https://github.com/portworx/px-rancher-extension.git`
   - **Git Branch**: `main`
4. Click **Create**.
5. Navigate to the **Extensions** page, and under the **Available** tab, you will see the Portworx extension. Install the latest version.

### Adding the Portworx Extension in an Air-Gapped Environment

For air-gapped environments, clone this repository into a private repository accessible to the Rancher cluster. Then, follow the steps above to add the extension to your Rancher UI.