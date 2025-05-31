# AWS VPC Base Module

A base module for a VPC on AWS.  Optionally can add a transit gateway.  This was created to demo module lifecycle management within HCP Terraform.  More in-depth documentation will be added later.

The required variables are:

- vpc_cidr_block (string)
- name (string)

If you'd like to make the VPC accessible from other ones via Transit gateway you'll need to add two other variables:

- transit_gateway_id (string)
- accessible_cidr_blocks (list of strings)

This VPC module was built to be used with other instances of it in a transit gateway pattern.

It can also optionally add IPv6 to the network but does not by default.

More docs to come later.