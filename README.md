# How to Deploy Network and Server Stack:

Important note: First we deploy Network stack. Then we will deploy Server Stack. Since Network stack has VPC, subnets (private and public), VPC NAT Gateway, Internet Gateway. The server stack is linked to the network stack. If you deploy server stack first then it will fail.

## Network Stack:

Type on command prompt/terminal:

`./create.sh ourinfra ourinfra.yml network-parameters.json`
 
If any changes are made to the network stack. Then run the following command:

`./update.sh ourinfra ourinfra.yml network-parameters.json`

# How to Deploy Server stack:

## Server Stack Deployment:

Type on command prompt/terminal:

 `./create.sh serverstack serverIAC.yml demoservers.json`
 
If any changes are made to the server stack. Then run the following command:
 
 `./create.sh serverstack serverIAC.yml demoservers.json`
