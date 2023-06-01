# Perform A/B testing and dark launches of your IoT applications using AWS IoT and Amazon CloudWatch Evidently
This solution demonstrates how Amazon CloudWatch Evidently can be used with AWS IoT Core and AWS Lambda to activate a feature flag embedded in your IoT application code, measure the impact of the new feature using controlled experiments, and use this information to launch the feature more widely across your fleet of devices.

## AWS Blog post
The AWS blog post explaining how this solution works, and how to deploy the Amazon CloudFormation templates.

TODO: Link to blog post

## Amazon CloudFormation templates
This repository provides the following Amazon CloudFormation templates used to provision the demo environment:

- `evidentlyIoT.yaml`
  - Provisions a stack housing the base infrastructure consisting of Amazon CloudWatch Evidently, AWS IoT Core and AWS Lambda resources. This can be used standalone to test the solution.
- `evidentlyIoTLoadGenerator.yaml`
  - Provisions an optional stack that deploys 50 test AWS IoT core devices. This is designed to allow you to demonstrate the running of Amazon CloudWatch Evidently experiments and launches at scale.


