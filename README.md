# Django example demo CI/CD pipeline


<a href="https://dash.elest.io/deploy?source=cicd&social=Github&url=https://github.com/elestio-examples/django"><img src="myapp\images\deploy-on-elestio.png" alt="Deploy on elest.io" width="180px" /></a>

Example application and CI/CD pipeline showing how to deploy a Django website to elestio.

<img src="myapp\images\django.png" alt="screenshot of the Django app" width="100%" />

## CI/CD on Elestio

Fork this repository to create your own copy that you can modify and use in a CI/CD pipeline


# Steps to create CI/CD pipeline on elestio

### Step 1: Select CI/CD from left sidebar in app.

Click [here](https://dash.elest.io/deploy?source=cicd) to directly go to the CI/CD

### Step 2: Select Deployment method.

We have three different types of deployment method

- Github
- Gitlab
- Docker compose

But for these Django website examples, you can choose GitHub as your deployment method.

### Step 3: Authentication

Select Clone in step at step Git Repository and select Django template for creating a repository in your git account after that authenticate with Git by clicking on Continue with Github button and authorize elestio to access git then you can rename you repository name if you want.

Else If you forked the repo then you can click on the Continue with GitHub button and authorize elestio to access the git repo then you can select the Django repo otherwise you can directly insert a git repo URL to deploy the Django App.

### Step 4: Configuration

After selecting a repo or inserting a URL it will auto-filled all the desired configurations using the elestio.yml/elestio.json file.

You can also manually customize the Configure your application, Reverse proxy configuration, and Environment variables.

### Step 5: Choose Deployment Targets

Elestio provides two different types of deployment targets.

- New Infrastructure
- Existing Infrastructures

On elestio single CI/CD target you can deploy multiple CI/CD pipelines so, If you already have CI/CD target on elestio then you can deploy a new pipeline on the same existing CI/CD target by choosing **Existing Infrastructures** and then select the CI/CD target otherwise if you don't have anything or want to deploy on new target then you can choose **New Infrastructure**

If you choose **New Infrastructure** then you have to select the deployment mode we have two different types of deployment modes.

- Single-mode.
- Cluster mode.

  **NOTE:-** Steps 6,7,8 and 9 are only for New Infrastructure targets for Existing Infrastructures targets directly following the final step.

### Step 6: Select Service Cloud Provider

Elestio supports five different types of cloud service providers you can choose anyone to deploy your service.

- Hetzner Cloud.
- Digital Ocean.
- Amazon Lightsail.
- Linode.
- Vultr.

We also provide a BYOVM service option so if you already have your VM on any third-party provider (Azure, GCP, Alibaba, ...) then you can choose BYOVM to deploy CI/CD pipeline on your VM.

Elestio provides one BYOVM service for free. To be eligible the VM you connect must have no more than 2 vCPU, max 4 GB of ram, and max 80 GB of storage

### Step 7: Select Service Plan

This step is only for other than BYOVM service providers.

We're providing multiple different types of service plans as per proposing by your selected providers.

### Step 8: Provide Service Name

By default, we create a unique target name for you but you can customize it.

### Step Final: Create Ci/CD pipeline

Now after following all the above steps you can click on the button **Create Ci/CD pipeline**.

It will take a few seconds to deploy your pipeline on elestio.

For each pipeline deployed on elestio will create a cname for it. but if you want your custom domain then you can configure it inside the target details.
