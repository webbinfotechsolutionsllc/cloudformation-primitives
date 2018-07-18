cloudformation-primitives
==================================
## Description

AWS best practice dictates the use of nested CloudFormation stacks wherever possible. The CloudFormation templates included here constitute reusable resource primitives which can be called as many times as desired from a root CloudFormation template.

AWS Cloudformation Documentation for nested stacks:

https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-nested-stacks.html

## Usage

Per AWS docs, these primitives must be referenced via an S3 URL by the root/parent stacks:

The URL of a template that specifies the stack that you want to create as a resource. Template files can use any extension, such as .json, .yaml, .template, or .txt. The template must be stored on an Amazon S3 bucket, so the URL must have the form: https://s3.amazonaws.com/.../TemplateName.extension

Author: Allan Webb

Email: awebb@witsolutions.com