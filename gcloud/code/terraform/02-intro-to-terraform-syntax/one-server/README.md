# Server Example

This folder contains an example [Terraform](https://www.terraform.io/) template that deploys a single server (using 
[Google Compute Engine](https://cloud.google.com/compute/) in a [Google Cloud Platform](https://cloud.google.com) account.

For more info, please see Chapter 2, "Getting started with Terraform", of 
*[Terraform: Up and Running](http://www.terraformupandrunning.com)*.

## Pre-requisites

* You must have [Terraform](https://www.terraform.io/) installed on your computer. 
* You must have an [Google Cloud Platform](https://cloud.google.com/) account.
* You must have downloaded a Google Cloud Platform credentials file.
* You must have enabled the Google Compute Engine API (CORRECT?)

Please note that this code was written for Terraform 0.9.x.

## Quick start

**Please note that this example will deploy real resources into your Google Cloud Platform account.
Check the [pricing](https://cloud.google.com/pricing/) and
[free trial](https://cloud.google.com/free/) pages.
We are not responsible for any charges you may incur.**

Configure GOOGLE_CREDENTIALS environment variable. The variable must contain the
*content* of the credentials file and not the path to it.

```
export GOOGLE_CREDENTIALS="$(cat ~/.gcloud/terraform-up-and-running-code-samples.json)"
```

Validate the templates:

```
terraform plan
```

Deploy the code:

```
terraform apply
```

Show the details.

```
terraform show
```

Clean up when you're done:

```
terraform destroy
```
