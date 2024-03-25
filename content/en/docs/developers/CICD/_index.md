---
title: "CICD"
linkTitle: "CICD"
weight: 8
date: 2022-03-14
description: >
    Detailed Explanation of Cloudforet CICD Pipeline and Architecture
no_list: true
---


## Actions
Cloudforet has 100+ repositories, **70 of which are for applications** and these repositories have github action workflows.

Because of that, it's very difficult to handle one by one when you need to update or run a workflow.

To solve this problem, we created `Actions`.<br>

The diagram below shows the relationship between Actions and repositories.

<img width="736" src="https://github.com/cloudforet-io/actions/assets/19552819/a8d490dd-2a6b-41ab-beb8-3dbf67c9a9d5">

### What does actions actually do?

`Actions` is a control tower that manages and deploys github action workflows for Cloudforet's core services.<br>
It can also bulk trigger these workflows when a new version of Cloudforet's core services needs to be released.

### 1. Manage and deploy github action workflows for Cloudforet's core services.
**All workflows for Cloudforet's core services are managed and deployed in this repository.**<br>

We write the workflow according to our workflow policy and put it in the [workflows](https://github.com/cloudforet-io/actions/tree/master/workflows/) directory of `Actions`.<br>
Then these workflows can be deployed into the repository of Cloudforet's core services

Our devops engineers can modify workflows according to our policy and deploy them in batches using this feature.

The diagram below shows the process for this feature.

<img width="935" src="https://github.com/cloudforet-io/actions/assets/19552819/755e8c71-42f8-4bf2-8a93-b83e13a839b3">


*) If you want to see the `Actions` script that appears  in the diagram, see [here](https://github.com/cloudforet-io/actions/tree/master/src).

### 2. trigger workflows when a new version of Cloudforet's core services needs to be released.
When a new version of Cloudforet's core services is released, we need to trigger the workflow of each repository.<br>
To do this, we made workflow that can trigger workflows of each repository in `Actions`.<br>

## Reference

[Cloudforet CICD Project, Actions](https://github.com/cloudforet-io/actions)
