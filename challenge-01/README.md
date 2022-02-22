# Terraform Challenge
The following challenge requires you to write a terraform project with self contained modules to do the following:

1) Create Two VPCs (10.100.0.0/16) and (10.101.0.0/16) under two different AWS accounts with the following subnets (/24)
dmz-00, dmz-01, app-00, app-01, db-00,db-01

- The DMZ subnets should be public and the rest should be internal subnets, all subnets need egress access to the internet. 
- VPC should include necessary IGs, Route Tables, NATs etc.
- 
2) Create a module that peers the two VPCS using terraform
Module should expose necessary routing tables etc, vpc peering ids etc.

3) Use aforemtioned module to peer the two VPCs together.
