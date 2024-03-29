# GitHub Recommended Settings

Overview

## Description

## Demo

## Features

### General

#### General

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/9d90dd95-94b4-49f9-987a-30fef1f6dafc)

- **Template repository**: `On`
- **Require contributors to sign off on web-based commits**: `On`
  - >"Require contributors to sign off on web-based commits" adds an additional layer of acknowledgment to commits made through the GitHub web interface. When contributors sign off on commits, they are essentially agreeing to certify that they have the right to submit the code and are licensing it under the project's open-source license.

#### Features

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/4a86cc54-5d41-434f-b2ba-2b4c9e343678)
![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/52bb6570-38bf-420a-b317-61e8a754a8b3)

- **Discussions**: `On`
  - >"Discussions" is a feature that allows community members to engage in threaded conversations directly within a repository. It's particularly useful for fostering collaboration, gathering feedback, and building a sense of community around your project.

#### Pull Request

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/404edc4e-5ace-420d-b493-b1b7fa480abb)

- **Allow rebase merging**: `Off`
  - >"Allow rebase merging" is a feature in GitHub that allows users to merge pull requests using the "Rebase and merge" option. Rebase merging is a technique where the changes in the pull request are applied on top of the latest changes in the target branch, resulting in a cleaner and linear commit history.
  - >By disabling rebase merging, GitHub will only allow traditional merge commits when merging pull requests. This can help maintain a more straightforward history and avoid any unintended consequences associated with rebase operations.

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/f26dc6f3-1f50-4a4e-923a-ed532c7a8a69)

- **Always suggest updating pull request branches**: `On`
  - >Enabling the "Always suggest updating pull request branches" setting in GitHub can be beneficial for keeping pull request branches up to date with changes in the base branch. When this setting is enabled, GitHub will automatically suggest updating the pull request branch when it becomes out of date with the base branch, typically due to new commits being added to the base branch.

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/f6c330f9-a03f-4149-a663-958a7707535d)

- **Automatically delete head branches**: `Off`
  - >By enabling this setting, GitHub will automatically delete head branches after pull requests are successfully merged, helping to keep your repository clean and organized.

#### Pushes

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/2ed08a3e-ca87-4e29-bfa9-c9d629669ff1)

- **Limit how many branches and tags can be updated in a single push**: `On`
  - >By enabling this setting, you can add an extra layer of protection to your repository and reduce the likelihood of accidental or unauthorized changes to multiple branches or tags in a single push operation. 

### Moderation options

#### Code review limits

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/5fa00423-154c-4d25-99d5-16cfe52b8800)

- **Limit to users explicitly granted read or higher access**: `On`
  - >By enabling this setting, you ensure that access to your repository is tightly controlled and restricted to only those users who have been explicitly granted read or higher access permissions. This helps protect sensitive information, maintain compliance with security standards, and reduce the risk of unauthorized access or data breaches. 

### Branches

- **Branch name pattern**: `main`

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/e8999e40-6734-44f4-9ed5-e671102f8ae9)

- **Dismiss stale pull request approvals when new commits are pushed**: `On`
  - >Enabling the "Dismiss stale pull request approvals when new commits are pushed" option in the "Require a pull request before merging" setting can be beneficial for maintaining the integrity and quality of your codebase. When this option is enabled, GitHub automatically dismisses stale pull request approvals whenever new commits are pushed to the branch associated with the pull request. This helps ensure that pull requests are reviewed against the latest changes and prevents outdated approvals from misleading the merge process.

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/4922dd92-d6c4-4241-913e-ccdb9e46fadb)

- **Require branches to be up to date before merging**: `On`
  - >Enabling the "Require branches to be up to date before merging" option in the "Require status checks to pass before merging" setting is generally a good practice, especially in collaborative development environments. When this option is enabled, GitHub ensures that the target branch of a pull request is up to date with the latest changes from the base branch before allowing the pull request to be merged. This helps maintain code consistency and prevents merging of outdated branches that may conflict with the latest changes in the base branch.

### Tags

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/f6fc3d43-8935-4398-a3a0-65139d1ef437)

- **Tag name pattern**: `[0-9].[0-9].[0-9]`
  - >Setting a "Tag name pattern" in GitHub can be helpful for enforcing a specific naming convention for tags, such as those used in semantic versioning. Semantic versioning typically follows the pattern major.minor.patch, where each component represents a different level of change in the software.

### Actions

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/ff033ee4-5159-4a5b-af5b-36b6b9e5ee99)

- **Actions permissions**: `Allow OWNER, and select non-OWNER, actions and reusable workflows`
- **Allow actions created by GitHub**: `On`
- **Allow actions by Marketplace verified creators**: `On`
  - >This setting allows repository owners to run actions and reusable workflows, as well as selected non-owners who are explicitly granted permission. It provides flexibility by allowing non-owners to access specified actions and workflows, which can be useful for collaborative projects where contributors need to execute certain tasks.

### Codespaces

#### Access and cost contro;

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/6ab91c3b-fe9b-4e35-a52c-878c4f7a4845)

- **Prebuild triggers**: `Configuration change`
  - >By selecting "Configuration change" as the prebuild trigger, you ensure that Codespaces automatically triggers a prebuild process whenever there is a change in the configuration files of your repository.
  - >Selecting "Configuration change" ensures that your Codespace environment is automatically updated whenever there is a change in configuration files such as Dockerfile, .devcontainer, or .codespace. This helps to keep your development environment consistent with the latest configuration settings, dependencies, and tooling specified in these files.
  - >Codespaces prebuilds your development environment based on the configuration files before you actually start using it. By triggering a prebuild on configuration changes, Codespaces ensures that any updates or modifications to the development environment are applied proactively, saving time and ensuring a smoother development experience.

### Code security and analysis

#### Dependabot

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/e9033919-5ffe-4f0c-834d-a4461ef29cb1)

- **Dependabot alerts**: `On`
  - >Dependabot alerts notify you when there are known security vulnerabilities in your project's dependencies, allowing you to promptly address them by updating to patched versions.

- **Dependabot security updates**: `On`
  - >Dependabot security updates automatically open pull requests to update vulnerable dependencies to their latest secure versions whenever security vulnerabilities are detected.

- **Dependabot version updates**: `On`
  - >Dependabot version updates automatically open pull requests to update your project's dependencies to their latest versions whenever new versions are available.

#### Code scanning

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/fd9840f5-5fc5-41aa-9454-920b5f3d4cf5)

Code scanning, powered by CodeQL, automatically analyzes your code for security vulnerabilities, coding errors, and other potential issues, providing actionable insights to help improve the overall security and quality of your software.

- **CodeQL analysis**: `Default`
  - >Enabling "Code scanning" with "CodeQL analysis" set to "Default" is a proactive approach to identifying and addressing potential security vulnerabilities and code quality issues in your codebase.

### Secret and variables

#### Repository secrets

![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/fa61b752-5cd7-407d-9d68-4aefaa731d06)
![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/eddc093d-12d5-4759-ac2e-08c3bb00ba4b)
![image](https://github.com/shinyay/github-recommended-settings/assets/3072734/f4891099-a78b-4b80-a722-5e54976b1864)


- **ACTIONS_RUNNER_DEBUG**: `true`
  - >"ACTIONS_RUNNER_DEBUG" is an environment variable that, when set to "true," enables debug logging for the self-hosted GitHub Actions runner. This can be useful for troubleshooting issues related to the execution of GitHub Actions workflows on self-hosted runners.
- **ACTIONS_STEP_DEBUG**: `true`
  - >"ACTIONS_STEP_DEBUG" is an environment variable that, when set to "true," enables debug logging for individual steps within GitHub Actions workflows. This can help you diagnose problems with specific workflow steps and identify issues with commands or scripts being executed.

## Requirement

## Usage

## Installation

## References

## Licence

Released under the [MIT license](https://gist.githubusercontent.com/shinyay/56e54ee4c0e22db8211e05e70a63247e/raw/34c6fdd50d54aa8e23560c296424aeb61599aa71/LICENSE)

## Author

- github: <https://github.com/shinyay>
- twitter: <https://twitter.com/yanashin18618>
- mastodon: <https://mastodon.social/@yanashin>
