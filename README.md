Task cat is used for automated testing of CloudFormation templates 

Overview:

Configured CodeBuild to run tests against the CloudFormation templates using CodePipeline


Run to Launch the Stack:

aws cloudformation create-stack --stack-name pipeline-taskcat --capabilities CAPABILITY_NAMED_IAM --disable-rollback --template-body file:///home/ec2-user/environment/taskcat-test/pipeline-taskcat.yml --parameters ParameterKey=GitHubUser,ParameterValue=nawinkumar94 ParameterKey=GitHubRepo,ParameterValue=taskcat-test

