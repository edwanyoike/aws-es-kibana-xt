[![npm version](https://badge.fury.io/js/aws-es-kibana.svg)](https://badge.fury.io/js/aws-es-kibana) ![dependencies](https://david-dm.org/santthosh/aws-es-kibana.svg)
[![Docker Stars](https://img.shields.io/docker/stars/santthosh/aws-es-kibana.svg)](https://registry.hub.docker.com/v2/repositories/santthosh/aws-es-kibana/stars/count/)

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/santthosh/aws-es-kibana)

# AWS ES/Kibana Proxy

AWS ElasticSearch/Kibana Proxy to access your [AWS ES](https://aws.amazon.com/elasticsearch-service/) cluster.

This is the solution for accessing your cluster if you have [configured access policies](http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-access-policies) for your ES domain

## Usage

Install the npm module

    npm install -g aws-es-kibana-xt
Set AWS credentials example below


     export AWS_ACCESS_KEY_ID="AIUDUBSUNSKDKSMKMKSNDKSDNSJ"
     export AWS_SECRET_ACCESS_KEY="sdefescvrefdc/casedfwedfwa"
     export AWS_REGION="eu-west-1"
     export ENDPOINT="search-xxxxx.us-west-2.es.amazonaws.com"


Run the proxy in two ways
1. aws-es-kibana-xt
2. aws-es-kibana-xt <cluster-endpoint> #if you had not set environment variable ENDPOINT

Example with hostname as cluster-endpoint:

aws-es-kibana-xt https://your-es-cluster-endpoint

### Run within docker container (under review)



## Credits

Adopted from this [gist](https://gist.github.com/nakedible-p/ad95dfb1c16e75af1ad5). Thanks [@nakedible-p](https://github.com/nakedible-p)
