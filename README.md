# aws-lambda-slsapp-sample-cloud9-demo 🐳

![Stars](https://img.shields.io/github/stars/tquangdo/aws-lambda-slsapp-sample-cloud9-demo?color=f05340)
![Issues](https://img.shields.io/github/issues/tquangdo/aws-lambda-slsapp-sample-cloud9-demo?color=f05340)
![Forks](https://img.shields.io/github/forks/tquangdo/aws-lambda-slsapp-sample-cloud9-demo?color=f05340)
[![Report an issue](https://img.shields.io/badge/Support-Issues-green)](https://github.com/tquangdo/aws-lambda-slsapp-sample-cloud9-demo/issues/new)

## reference
[youtube](https://www.youtube.com/watch?v=mIky1niHGdY)

## lambda
- name=`dtq-lambda-slsapp`
![lambda1](screenshots/lambda1.png)
---
![lambda2](screenshots/lambda2.png)
---
![lambda3](screenshots/lambda3.png)

## ec2
- name=`aws-cloud9-DTQCloud9LambdaSLSApp-...`
![ec2](screenshots/ec2.png)

## dynamodb
- name=`dtq-lambda-slsapp-SampleTable--...`
![dynamodb](screenshots/dynamodb.png)

## cloudformation
![cf](screenshots/cf.png)

## pipeline
![pipeline](screenshots/pipeline.png)

## cloud9
- name=`DTQCloud9LambdaSLSApp`
- auto created `/dtq-lambda-slsapp/template.yml`
![yaml](screenshots/yaml.png)
- `git clone codecommit://dtq-lambda-slsapp && cd dtq-lambda-slsapp` 
- `curl https://iadi4xvera.execute-api.us-east-1.amazonaws.com/Prod/xxx` -> see nothing
- edit `bodyString` variable in `get-by-id.js`
![get-by-id](screenshots/get-by-id.png)
```shell
git add --all
git commit -m "1st"
git push
```
- after CICD finished, `curl https://iadi4xvera.execute-api.us-east-1.amazonaws.com/Prod/xxx` -> see:
```json
{"err": "KO thay!!!"}
```
