# spring-gumball

### This example demonstrates the following two GitHub Workflows.

* https://help.github.com/actions/language-and-framework-guides/building-and-testing-java-with-gradle

* https://github.com/google-github-actions/setup-gcloud/tree/master/example-workflows/gke

### Build Dependencies

* Gradle 5.6
* JDK 11

<h2>CI Workflow</h2>

main.yml in ./github/workflows:
![](screenshots/CI-workflow4.png)

After committing to main branch:
![](screenshots/CI-workflow1.png)
![](screenshots/CI-workflow2.png)
![](screenshots/CI-workflow3.png)

<h2>CD Workflow</h2>

Create IAM account with roles Kubernetes Engine Developer and Storage Admin:
![](screenshots/CD-IAMaccount.png)

Create service account and secret key:
![](screenshots/CD-serviceaccount.png)
![](screenshots/CD-jsonsecret.png)

Github secrets:
![](screenshots/CD-gitsecrets.png)

Github release:
![](screenshots/CD-release.png)

Github actions:
![](screenshots/CD-gkebuild.png)

GKE deployment:
![](screenshots/CD-deployment.png)

GKE service:
![](screenshots/CD-service.png)

GKE ingress:
![](screenshots/CD-ingress.png)

Spring Gumball:
![](screenshots/CD-frontend.png)
