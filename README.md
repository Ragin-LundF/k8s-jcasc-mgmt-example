# k8s-jcasc-mgmt-example

This repository is an example project for [k8s-jcasc-management-go](https://github.com/Ragin-LundF/k8s-jcasc-management-go) or [k8s-jcasc-management](https://github.com/Ragin-LundF/k8s-jcasc-management) together with the [jenkins-jobdsl-remote](https://github.com/Ragin-LundF/jenkins-jobdsl-remote) tool.

In a regular project, please do not combine both things together and create separate repositories for the job definitions!
This means, that the directories:
- config
- projects
- templates

should be an own repository and the `jenkins-dsl-jobs.json` should be another repository.

The `jenkins-dsl-jobs.json` file should be under control of the project developers, and the previously mentioned directories should be under the control of the DevOps.

In the `templates` directory is a copy of the original one and contains new/customized templates in the `cloud-templates` directory.
If you want to use own or modified templates, you have to copy all of them into this directory, which is then under your control.

The `projects` folder contains two examples of projects:

- `example-project` is a project with saved value files, which can be modified manually
- `example-project-dynamic` is a project which contains only the JCasC and the configuration file.
  The Helm values files are generated on-the-fly from the configuration.

More information:
- Medium Article [Kubernetes and CI/CD — How to integrate in your development process](https://ragin.medium.com/kubernetes-and-ci-cd-how-to-integrate-in-your-development-process-9b483b194975)
- Github [k8s-JCasC-Mgmt tool](https://github.com/Ragin-LundF/k8s-jcasc-management-go)
- Github [k8s-JCasC-Mgmt example project](https://github.com/Ragin-LundF/k8s-jcasc-mgmt-example)
- Github [k8s-JCasC-app-example](https://github.com/Ragin-LundF/k8s-jcasc-app-example)
- Github [k8s-JCasC docker containers](https://github.com/Ragin-LundF/k8s-jenkins-docker)
- Github [k8s-JCasC helm charts example](https://github.com/Ragin-LundF/k8s-jcasc-app-helm-charts)
- Github [k8s-JCasC helmfile deployment example](https://github.com/Ragin-LundF/k8s-jcasc-deploy-helmfile-example)
