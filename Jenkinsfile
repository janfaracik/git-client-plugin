#!/usr/bin/env groovy

/* `buildPlugin` step provided by: https://github.com/jenkins-infra/pipeline-library */
buildPlugin(
  // Container agents start faster and are easier to administer
  useContainerAgent: true,
  // Show failures on all configurations
  failFast: false,
  // Test Java 11 with default release, Java 17 with more recent
  configurations: [
    [platform: 'linux',   jdk: '11'], // Linux first for coverage report on ci.jenkins.io
    [platform: 'windows', jdk: '17', jenkins: '2.389']
  ]
)
