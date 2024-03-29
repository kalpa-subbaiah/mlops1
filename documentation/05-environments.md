# Work with environments

There are many advantages to using environments in machine learning projects. When you have separate environments for development, staging, and production, you can more easily control access to resources. 

Use environments to isolate workloads and control the deployment of the model.

## Prerequisites

If you haven't, complete the [set-up](00-set-up.md) before you continue. **Your repo should be set to public**. If you're using a private repo without GitHub Enterprise Cloud, you'll not be able to create environments. [Change the visibility of your repo to public](https://docs.github.com/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility) if your repo is set to private.

You'll also need the GitHub Action that triggers the Azure Machine Learning pipeline created in Challenge 3. 

## Learning objectives

By completing this challenge, you'll learn how to:

- Set up a development and production environment.
- Add environments to GitHub Action.
- Add a required reviewer to the staging job environment.

## Tasks

Though it's a best practice to associate a separate Azure Machine Learning workspace to each environment, you can use one workspace for both the development and production environment for this challenge. 

- Within your GitHub repo, create a development and production environment.
- Add an approval check for the production environment.  
- Create one GitHub Actions workflow that trains the model in the development environment and downloads the last job's output in the production environment.

## Success criteria

To complete this challenge successfully, you should be able to show:

- A successfully completed Actions workflow in your GitHub repo that trains the model and downloads the job's output.
- Show that the workflow required an approval before running the production workload.

## Useful resources

- [Learning path covering an introduction of DevOps principles for machine learning.](https://docs.microsoft.com/learn/paths/introduction-machine-learn-operations/)
- [GitHub Actions.](https://docs.github.com/actions/guides)
- [Using environments for deployment in GitHub.](https://docs.github.com/actions/deployment/targeting-different-environments/using-environments-for-deployment)