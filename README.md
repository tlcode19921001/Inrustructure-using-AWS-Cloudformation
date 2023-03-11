# Inrustructure using AWS Cloudformation

This repository containes CloudFormation template and Ansible roles.

## CloudFormation

This template includes:

* VPC
* PublicSubnet
* Internet Gateway
* EC2 SecurityGroup
* CloudWatchAccessProfile
* Elastic IP
* EC2 instance with two EBS attached

## Ansible

Used to run CloudFormation and roles to install and configure services:

* common (configure EC2 hostname, users etc)
* cloudformation (create or update CloudFormation stack)
* letsencrypt (install client, obtain SSL certificates, add a cronjob for renewal)
* mysql (MariaDB installation, create users/databases etc)
* nginx (install, copy virtual hosts configs etc)
* php-fpm (install, configure FMP-pools)
