## Portworx Rancher extension
Portworx is a software-defined storage solution that ensures high availability for containerized stateful applications across multiple nodes and cloud environments. It facilitates seamless workload migration between clusters, supports hyperconverged deployments by co-locating data and applications, and offers programmatic control over storage resources.
This extension integrates Portworx storage monitoring directly within the Rancher dashboard.
### Prerequisites
- Supported Kubernetes version: 1.16.0 or later
- Supported Rancher version: 2.7.0 or later
- You must be logged in as an admin to add and install the Portworx extension to the Rancher dashboard.
### Install Portworx extension
Follow the steps below to install the Portworx Rancher extension:
1. Navigate to **☰ > Extensions** in the Rancher UI.
2. In the top-right corner, click **⋮ > Manage Repositories > Create**.
3. Provide the following details:
   - **Name**: Enter a name for your Portworx Rancher repository.
   - Select the **Target** as **Git repository containing Helm chart or cluster template definitions**.
   - **Git Repo URL**: `https://github.com/portworx/px-rancher-extension.git`
   - **Git Branch**: `main`
4. Click **Create** to add the repository.
5. Go to the **Available** tab and locate the Portworx extension.
6. Click **Install** on the desired version.
7. After installation, click the **Reload page** button to update the UI.  
   > **Note:** UI changes will not reflect until you reload the page.
### Update Portworx extension
Follow the steps below to update your Portworx Rancher extension:
1. Navigate to **☰ > Extensions** in the Rancher UI.
2. Go to the **Updates** tab.
3. Click **Update** if a new version is available.  
   Alternatively, check the **Available** tab for the extension. If an update is available, an **Update** button will appear on its card.
4. After upgrading, click the **Reload page** button to update the UI.  
   > **Note:** UI changes will not reflect until you reload the page.
### Uninstall Portworx extension
Follow the steps below to remove the Portworx Rancher extension:
1. Navigate to **☰ > Extensions** in the Rancher UI.
2. Under the **Installed** tab, find the Portworx extension.
3. Click **Uninstall**.
4. After the extension is removed, click the **Reload page** button to refresh the UI.
   > **Note:** UI changes will not reflect until you reload the page.
### Install Portworx extension in an Air-gapped environment
For air-gapped environments, clone this repository into a private repository accessible to the Rancher cluster. Then, follow the steps in [Install Portworx extension](#install-portworx-extension).
### Limitations
Portworx Rancher extension is not supported on PX-Security enabled clusters.