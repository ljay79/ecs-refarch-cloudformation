- Add ENVIRONMENT Param for use as ressource name prefix instead of using StackName (test,staging,production)
- add EC2 with MySQL instance template with retention policy:retain
- attach optional Bastion instance from foreign VPC?!
- application/apache logging to CloudWatch (check already implemented Sample logging)
- hardening ECS securitygroups / access to any resources / ACL / ...
- define apps services based on sample according to our real needs
- check dependencies between apps (crm <-> dashboard <-> frontend) like internal calls, urls, ...?
-- for stack requirements
- restructure/adjust CF template organization and references, take them out of app/services code bases
- parameterize VPCs and subnet cidr range (10.10.xx.xx, 10.20.xx.xx, ..) make optional and keep default from sample

- branch out a version with minimal Ressources and availabilities (singe AZ, single ECS cluster, ...)

- find autom way (bitbucket pipeline) to update private S3 bucket with CloudFormation templates, as CF can use/reference only S3 locations
