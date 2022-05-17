# spring-gumball

### This example demonstrates the following two GitHub Workflows.

* https://help.github.com/actions/language-and-framework-guides/building-and-testing-java-with-gradle

* https://github.com/google-github-actions/setup-gcloud/tree/master/example-workflows/gke

### Build Dependencies

* Gradle 5.6
* JDK 11

<h2>CI Workflow</h2>

main.yml in ./github/workflows:
![](screenshots/CI-workflow1.png)

After committing to main branch:
![](screenshots/CI-workflow.png)

<h2>CD Workflow</h2>

Create GKE service account with secret key:
![](screenshots/CD-gkeaccounts.png)
![](screenshots/CD-gkekey.png)

Add project ID and key to Action Secret:
![](screenshots/CD-actionsecrets.png)

Ran into errors because of incorrect permissions in GKE:
![](screenshots/CD-workflowerror.png)

Configuring proper permissions:
![](screenshots/CD-projectpermissions.png)

After creating a release:
![](screenshots/CD-gkeworkflow.png)

Project deployed on GCP:
Cluster -
![](screenshots/CD-service.png)

Workload - 
![](screenshots/CD-workload.png)

Service - 
![](screenshots/CD-service.png)

Ingress - 
![](screenshots/CD-ingress.png)

Gumball running on endpoint:
![](screenshots/CD-gumball.png)



