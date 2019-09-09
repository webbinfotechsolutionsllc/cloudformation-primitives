cloudformation-primitives
==================================
## Description

AWS best practice dictates the use of nested CloudFormation stacks wherever possible. The CloudFormation templates included here constitute reusable resource primitives which can be called as many times as desired from a root CloudFormation template.

AWS Cloudformation Documentation for nested stacks:

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-nested-stacks.html

## Usage

Per AWS docs, these primitives must be referenced via an S3 URL by the root/parent stacks:

The URL of a template that specifies the stack that you want to create as a resource. Template files can use any extension, such as .json, .yaml, .template, or .txt. The template must be stored on an Amazon S3 bucket, so the URL must have the form: https://s3.amazonaws.com/.../TemplateName.extension

## Parent Example

The parent_ec2_vpc.yaml template is an example parent template using nested CloudFormation primitives to create a complete set of resources necessary for a functional VPC, including the VPC itself, IGW, public and private subnets, Route Tables, DHCP Option set, etc. In this case, the parent template assumes three AZs with one public and one private subnet in each.

Author: Allan Webb

Email: awebb@witsolutions.com