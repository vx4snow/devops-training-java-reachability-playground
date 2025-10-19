Assignment to create End to End DevSecOps Repo for .NET/C# Project
Assignment Title: Create an End to End DevSecOps pipeline using GitHub Actions for a C# application

Description: In this task, you need to create a DevSecOps pipeline with the following stages:

1) Stage One should run SonarCloud analysis on the source code

2) Stage Two should run SCA analysis using Snyk

3) Stage Three should run DAST scan on "http://example.com"



The following GitHub URL contains the C# application for which we need to implement an End to End DevSecOps pipeline using GitHub Actions workflow.

Assignment - Sample application of C# for implementing an End to End DevSecOps Pipeline using GitHub Actions



Solution of this assignment is present in the following repo. But please only look into this solution after implementing the Github actions workflow:

Solution - Sample application of C# for implementing an End to End DevSecOps Pipeline using GitHub Actions



The solution repo contains workflow file with SAST, SCA and DAST steps added to the "devsecops-workflow.yaml" file. This workflow file contains End to End implementation of DevSecOps pipeline for C# project.



-----

Some Common Errors and their solutions
If you are facing the below error while running DAST scan using GitHub Actions:






Solution to this problem is:

In your Github actions workflow file for OWASP ZAP code, make sure your branch name is correct. For example, in the following screenshot, the highlighted name should be the same as your branch name. If not, your DAST scan will fail.








Note: Also, make sure you are not running DAST scan on a cloned repo. DAST scan should be run from a fresh repo.

