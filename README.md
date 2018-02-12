## Overview
This repo contains a [Dockerfile](Dockerfile) that runs Jenkins inside a Docker
container and uses [Nginx][nginx-home] as a reverse proxy. It also provides
several Jenkins plugins and a basic Jenkins configuration in order to get you
up and running quickly with Jenkins on DC/OS.

This repo is a fork of https://github.com/mesosphere/dcos-jenkins-service, the 
official DCOS Jenkins service. The purpose for this repo is to quickly 
enable `rspec`, `puppet-lint`, and `puppet-syntax` testing of Puppet modules using
Pipelines. This fork achieves this by installing `RVM`, `Ruby`, and all `gems` 
required for Puppet module testing.


## Included in this repo
Base packages:
  * [Jenkins][jenkins-home] 2.89.2 (LTS)
  * [Nginx][nginx-home] 1.10.1

Jenkins plugins:
  * ant v1.7
  * ace-editor v1.1
  * ansicolor v0.5.2
  * antisamy-markup-formatter v1.5
  * artifactory v2.13.1
  * authentication-tokens v1.3
  * azure-vm-agents v0.5.0
  * blueocean v1.3.5
  * branch-api v2.0.16
  * build-name-setter v1.6.7
  * build-timeout v1.19
  * cloudbees-folder v6.2.1
  * conditional-buildstep v1.3.6
  * config-file-provider v2.16.4
  * copyartifact v1.39
  * cvs v2.13
  * docker-build-publish v1.3.2
  * docker-workflow v1.14
  * durable-task v1.17
  * ec2 v1.38
  * embeddable-build-status v1.9
  * external-monitor-job v1.7
  * ghprb v1.39.0
  * git v3.6.4
  * git-client v2.6.0
  * git-server v1.7
  * github v1.28.1
  * github-api v1.90
  * github-branch-source v2.3.1
  * github-organization-folder v1.6
  * gitlab v1.5.2
  * gradle v1.28
  * greenballs v1.15
  * handlebars v1.1.1
  * ivy v1.28
  * jackson2-api v2.8.10.1
  * job-dsl v1.66
  * jobConfigHistory v2.18
  * jquery v1.12.4-0
  * ldap v1.18
  * mapdb-api v1.0.9.0
  * marathon v1.6.0
  * matrix-auth v2.2
  * matrix-project v1.12
  * maven-plugin v3.0
  * mesos v0.15.0
  * metrics v3.1.2.10
  * momentjs v1.1.1
  * monitoring v1.70.0
  * nant v1.4.3
  * node-iterator-api v1.5.0
  * pam-auth v1.3
  * parameterized-trigger v2.35.2
  * pipeline-build-step v2.6
  * pipeline-github-lib v1.0
  * pipeline-input-step v2.8
  * pipeline-milestone-step v1.3.1
  * pipeline-model-definition v1.2.5
  * pipeline-model-extensions v1.2.5
  * pipeline-rest-api v2.9
  * pipeline-stage-step v2.3
  * pipeline-stage-view v2.9
  * plain-credentials v1.4
  * rebuild v1.27
  * role-strategy v2.6.1
  * run-condition v1.0
  * s3 v0.10.12
  * saferestart v0.3
  * saml v1.0.4
  * scm-api v2.2.6
  * ssh-agent v1.15
  * ssh-slaves v1.23
  * subversion v2.10.1
  * timestamper v1.8.8
  * translation v1.15
  * variant v1.1
  * windows-slaves v1.3.1
  * workflow-aggregator v2.5
  * workflow-api v2.24
  * workflow-basic-steps v2.6
  * workflow-cps v2.42
  * workflow-cps-global-lib v2.9
  * workflow-durable-task-step v2.17
  * workflow-job v2.16
  * workflow-multibranch v2.16
  * workflow-scm-step v2.6
  * workflow-step-api v2.14
  * workflow-support v2.16
