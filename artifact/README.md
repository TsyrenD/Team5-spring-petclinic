create main.tf and provider.tf
in google go to "Google Cloud Platform Provider - hashicorp"
Copy
# provider "google" {
#   project     = "my-project-id" >> fit-symbol-382321
#   region      = "us-central1"
# }
Go to "google_artifact_registry_repository | Resources | hashicorp ..."
COPY
# resource "google_artifact_registry_repository" "my-repo" {
#   location      = "us-central1"
#   repository_id = "my-repository" >> "spring-clinic"
#   description   = "example docker repository" >> "spring-clinic docker repository"
#   format        = "DOCKER"
# }
PASTE in main.tf
terraform init
terraform apply -auto-approve
terrform destroy
docker > open integrate terminal
COPY from repository "spring-clinic"
# gcloud auth configure-docker \
#     us-central1-docker.pkg.dev
in docker terminal
# gcloud artifacts locations list > this command show what  region avaible
# git checkout -b 2.0.0 > create new branch
# git checkout 2.0.0 > go to branch 2.0.0
# docker build -t us-central1-docker.pkg.dev/fit-symbol-382321/spring-clinic

