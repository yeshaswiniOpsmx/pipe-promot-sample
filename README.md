Sample repo to show pipeline-promotion functionality. The repo shows at a stage where pipelineSyncToGit stage has been executed against a "source" spinnaker.
Each application data is stored in a folder with the application-name. Each pipeline is stored in file with the pipeline-name.json. Application-json is also stored and is created by default, if not present, in the target Spinnaker. pipelines_in_application.list is a file with a list of all pipelines that is used for internal purposes.

opsmx-gitops application and pipelines also help as helper pipelines in for gitops-style Spinnaker installation.

default-config directory in srinipipepromot application is created automatically, based on pipeconfigcreate flag=true.

prod-config directory is a sample directory where parameter files are processed and pipeline updated for another environment e.g. prod. File-names need to be same as the pipeline file-names. Simplest way is to copy the file from default-config, edit as desired, and check it into prod-config.
