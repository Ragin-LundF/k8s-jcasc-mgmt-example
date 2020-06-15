# k8s-jcasc-mgmt-example

This repository is an example project for [k8s-jcasc-management-go](https://github.com/Ragin-LundF/k8s-jcasc-management-go) or [k8s-jcasc-management](https://github.com/Ragin-LundF/k8s-jcasc-management) together with the [jenkins-jobdsl-remote](https://github.com/Ragin-LundF/jenkins-jobdsl-remote) tool.

In a regular project, please do not combine both things together and create seperate repositories for the job definitions!
This means, that the directories:
- config
- projects
- secrets

should be an own repository and the `jenkins-dsl-jobs.json` should be an own repository.

The `jenkins-dsl-jobs.json` file should be under control of the project developers, and the previously mentioned directories should be under the control of the DevOps.

In a real project, it can also be necessary to add the `templates` directory with own templates.