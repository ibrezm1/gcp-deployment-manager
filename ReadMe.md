## Important links
* [Google Quickstart](https://cloud.google.com/deployment-manager/docs/manage-cloud-resources-deployment)
* [Google Git Sample](https://github.com/GoogleCloudPlatform/deploymentmanager-samples/blob/33f4cb46e9980811c0d5a8f14f2f514efb4a8abc/examples/v2/build_configuration/vm.yaml)
* [Google Docs](https://cloud.google.com/deployment-manager/docs/configuration)

## Commands 
* gcloud config set project
* gcloud deployment-manager deployments create quickstart-deployment --config vm.yaml
* Check status here 
    * gcloud deployment-manager deployments describe quickstart-deployment
* Update deployment 
    * gcloud deployment-manager deployments update example-deployment \
    --config configuration-file.yaml \
    --preview
    * gcloud deployment-manager deployments update example-deployment
* gcloud deployment-manager deployments delete quickstart-deployment
* List all images 
    * gcloud compute images list --uri( Check Family )
    * gcloud compute disks create my-disk-1 --source-disk old_disk --zone=us-east1-a