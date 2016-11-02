# ec2-tags-env

**This script is written for my personal usage, and may not be suitable to use in a production environment.**

import-tags - Import your AWS EC2 (instance and IAM) tags as Shell environment variables. (all tags as vars)

import-tag - This script will export a base-64 encoded list of vars under the tag named "envVars" 

## Requirements

- jq package https://stedolan.github.io/jq/
- AWS CLI tool https://github.com/aws/aws-cli (probably already installed in your AMI)
- IAM policy allowing you to use `ec2:DescribeTags`

## Usage

    . ./import-tags.sh
    
   or 
 
    . ./import-tag.sh