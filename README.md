# Introduction to Terraform

This repository is all of the material that was used for [my talk](https://embed.pheedloop.com/dodto19/site/sessions/?id=KzXXQA) at DevOpsDays Toronto 2019.

## Scenario

You -- an intrepid infrasturucture engineer -- have been tasked with a green field application project on AWS. The team decided that embracing the codification of infrastructure as well as the applicaiton itself was crucial.

Two crucial problems:
1. Nobody on the team has codified infrastructure before
1. Despite having crafted a bang up whiteboard diagram, going from the picture to code feels like looking over the edge into the abyss.

## Structure

Each "milestone" directly is intended to be a stepping stone of increased proficiency and complexity as we move toward our goal state: 

![Desired End State](images/milestone-4.png)

## Requirements

* Terraform 0.12.0+ installed
* An AWS account
  * I've tried my best to use [free tier](https://aws.amazon.com/free/) eligible or low-cost service options

The [AWS provider](https://www.terraform.io/docs/providers/aws/index.html) is currently configured in such a way that it expects your environment to have appropriate [environment variables](https://www.terraform.io/docs/providers/aws/index.html#environment-variables) configured or have setup the AWS CLI with a default or named profile [configured](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html).

## Usage

As each "milestone" directory is intended to be moved through in sequence as the environment becomes more flushed out and the usage of Terraform slightly more complicated.

Beginning in "milestone-1" directory, the README will display a diagram of the intended milestone of that iteration. Executing `terraform plan` will show you the resources that need to be created. `terraform apply` will create the resources.
