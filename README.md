# Cloud-Security

AWS security strategy and architecture 

top down security design

secure the organization

secure the ogranization OU

Secure the account

Secure the network

Secure the orgnization & OU will include security Hub, control tower, SCP, SSO, Cloudtrail, Firewall Manager, IAM advisor, etc

Scure the account level, will have SCP, cloudtrail, AWS config, System Manager, Guardduty, Inspector, Security Hub, IAM access advisor and cloudwatch

Scure the network will have inspector, WAF, shield, FW, FW manager, ACM, SG, NACL, GW, VPC endpoints, endpoint policy, flow logs, traffic monitoring


AWS compliance and assurance

Four layers of compliance and assurance

layer 1: AWS config set up the standard compliance rules, collect the aggregated account config data, update the AWS security hub, control torwe, and backup 
layer 2: Sydtem manager do the image and patch management, pre-built the image for the VM/container
Layer 3: AWS auditing Manager integrate with cloudtrail, provided pre-built automatic generated compliance reports for auditing
layer 4: confirmation guard provide the guardrail for the code check before the resource provision. 


Best Practice of the security design

1. IdP with federated SSO with IAM, SCP 
2. Enable the traceability 
3. Apply security at all layers
4. Automate security best practice
5. Pretent Data in transit and rest
6. use SCP and IAM to keep the data away
7. Security event automation 
8. security hub built-in compliance PCI-DSS, use it. Security hub integrated with guardduty, inspector, miace, IAM access analyzer, firewall manager, central view
9. CMK(customer Master Key) customer managed VS AWS managed retain period different
10. SCP deny permit deny rules on the organization level together with IAM and resource based policy to control the resource access and creation
11. always use session manager/SSM as default for private VPC instance access
12. deny the S3 and other resource public access
13. enable the auto backup 

