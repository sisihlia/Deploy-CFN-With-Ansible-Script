# Deploy-CFN-With-Ansible-Script


Deploy cloudfront.yaml

aws cloudformation deploy \
--template-file cloudfront.yaml \
--stack-name production-distro \
--parameter-overrides PipelineID="${S3_BUCKET_NAME}" \ # Name of the S3 bucket you created manually.
--tags project=udapeople &
