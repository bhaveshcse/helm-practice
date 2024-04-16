# Helm
Helm is an open-source graduated CNCF project originally created by DeisLabs as a third-party utility, now known as the package manager for Kubernetes, focused on automating the Kubernetes applications lifecycle in a simple and consistent way.

The objective of Helm as package manager is to make an easy and automated management (install, update, or uninstall) of packages for Kubernetes applications, and deploy them with just a few commands.

## Why use Helm?
Deploying your applications manually seems complex without using Helm. You will have to define every single YAML configuration, from configuring your workloads to how (and what) you want them to be deployed. And it’s not only that. After defining and debugging the YAML, think about what will happen after updating the application? You will have to manually remove all created resources and re-deploy them for the new version, which can be slightly mitigated if you create additional files for automation, but that costs additional effort.

Helm is the simplification of this. With Helm, you can simply download your preferred Helm chart, deploy it in the cluster, and update or delete it with low effort. Helm means several benefits for your application:

  1. Offers Helm charts and repositories where you get everything necessary for deployment and its configurations.
  2. Official Helm charts are up to date and maintained with new releases.
  3. Allows you to jump between your preferred versions of the Helm chart.
  4. Everything with just a single CLI command.

# Helm installation on Ubuntu
```bash
curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
sudo apt-get install apt-transport-https --yes
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
sudo apt-get update
sudo apt-get install helm
```
# Helm cheat sheet
https://helm.sh/docs/intro/cheatsheet/
