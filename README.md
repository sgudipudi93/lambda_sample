This is a sample S3 website created using Lambda

**Deployment Steps:**
```
1) Create a bucket named "sgudipudi-code"
2) aws cloudformation package --s3-bucket sgudipudi-code --template-file ./template.yaml --output-template-file ./template-packaged.yaml
3) aws cloudformation deploy --stack-name sgudipudiwebsite --template-file ./template_packaged.yaml --capabilities CAPABILITY_IAM
```