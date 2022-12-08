

![subnets creation](./public & private subnets being created.png)

# Tag your resources

![tagging introduced](./tagging of resources.png)

# Create Natgateway

Note that natgateway depends on the elastic IP. Also, natgateway and elastic IP depends on internet gateway. Hence, "internet gateway" should be created before elastic IP and natgateway.

Also, do not fail to declare all variables in the variables.tf and declare the values in terraform.tfvars.

![creation of other resources](./creation of int-gw, nat-gw & EIP.png)


## Install graphviz sudo apt install graphviz
## terraform graph -type=plan | dot -Tpng > graph.png
## terraform graph | dot -Tpng > graph.png
## https://www.terraform.io/docs/cli/commands/h=graph.html


# Create route tables and routes.
Note that the route determines the path or flow of traffic.

![route tables created](./creation of public & private route tables.png)

Run "terraform apply --auto-approve" to apply what you've created.


