# CI/CD

- [CI/CD](#cicd)
  - [About](#about)
  - [Jenkins](#jenkins)
    - [Agents](#agents)
  - [Forgejo](#forgejo)
    - [Webhooks](#webhooks)

## About

Covers my pipelines for personal programming projects.

## Jenkins

I use Jenkins to test and deploy my projects. Mostly automated through webhooks to autodeploy based on git pushes. Jenkins may be much for a home server like this but I had learned it through my schooling and thought it would be a fun project.

### Agents

I use Jenkins agents to perform the tasks I assign them in pipelines. This is deployed through a container aswell so management is the same as all my other apps but it has access to the host machine.

## Forgejo

I run a localized git server using Foregjo. Nothing fancy and is almost identical to Github. It is used for personal projects that aren't meant to be public. If I do want to make a repo public, I simply will mirror the main branch of a project to a public Github repo.

### Webhooks

I use web hooks in Forgejo to trigger processes in Jenkins. For example when I push to main for my [portfolio](https://benmacintyre.net), it will rebuild and deploy an apache container on the server.