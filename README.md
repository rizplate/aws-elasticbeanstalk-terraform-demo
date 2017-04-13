# Elastic Beanstalk, Docker and Terraform

First: There a [full blog post](https://flypenguin.de/2017/04/13/elastic-beanstalk-with-docker-using-terraform/) about this repo. Read it for a more detailed info.


## Quickstart

* copy `terraform.tfvars.dist` to `terraform.tfvars` and fill in your own values
* run `terraform plan` to see what would happen
* run `terraform apply` to get the application and an environment
* run `app_config_create_and_upload.sh` to create an application version
* run `terraform plan` (and `apply` after) to get the version deployed
* run `deploy.sh` to actually deploy the version into the created environment

## Notes

* Single container app only
* Uses the image `flypenguin/test` by default, which can simulate load
* No private repos
