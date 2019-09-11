# DevOps PlayGround
Project to play around with Azure DevOps.

The Git workflow follows the "Release Flow" as used by Microsoft and described in https://docs.microsoft.com/en-us/azure/devops/learn/devops-at-microsoft/release-flow

With Azure DevOps CI implemented - every commit (without PRs) to branch "master" will be compiled and deployed to slot "dev" in Azure Web App https://devopsplayground-dev.azurewebsites.net/
Every branch name like 'releases/...' will trigger a compilation and deployment to slot "release" in Azure Web App https://devopsplayground-release.azurewebsites.net

Works with .NET Core 3.0 (Preview), see https://chamindac.blogspot.com/2019/08/build-net-core-30-projects-with-azure.html for hints to get this up an running.
