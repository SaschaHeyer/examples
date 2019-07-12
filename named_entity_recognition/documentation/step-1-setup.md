# Setup

## Deploying Kubeflow to Google Cloud Platform
This example requires a running Kubeflow environment (v0.5.0). The easiest way to setup a Kubeflow environment is by using the [Deployment UI](https://www.kubeflow.org/docs/gke/deploy/deploy-ui/).

## Create bucket
Create a bucket, this bucket will contain everything which is required for our Kubeflow pipeline. 

```bash
gsutil mb -c regional -l us-east1 gs://your-bucket-name
```

## Set enviornment variables

Create the following environment variables, follow the [documenation](https://cloud.google.com/resource-manager/docs/creating-managing-projects#identifying_projects) to get the project id :

```bash
export BUCKET=your-bucket-name
export PROJECT_ID=your-gcp-project-id
```

## Clone this repository
Clone the following repository, it contains everything which is needed for this example.

```bash
git clone https://github.com/kubeflow/examples.git
```

Open a Terminal and navigate to the folder `/examples/named-entity-recognition/`.

*Next*: [Build the pipeline components](step-2-build-components.md)