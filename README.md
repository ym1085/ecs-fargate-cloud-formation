# ECS Fargate CloudFormation Template Sample

> Sample to conduct cloudformation test

## Package Structure

```bash
ECS-FARGATE-CLOUD-FORMATION - root project
  ├── templates
  │   ├── compute                     # Compute resources related to ECS
  │   │   ├── ecs_cluster.yaml        # Defines the ECS cluster
  │   │   ├── service.yaml            # Defines the ECS service
  │   │   └── task_definition.yaml    # Defines the ECS task definition
  │   ├── env                         # Environment-specific stack definitions
  │   │   ├── dev                     # Development environment stack
  │   │   │   └── main.yaml           # Full stack definition for the dev environment
  │   │   └── prod                    # Production environment stack
  │   │       └── main.yaml           # Full stack definition for the prod environment
  │   ├── iam                         # IAM roles and policies definitions
  │   │   ├── policies.yaml           # Defines IAM policies
  │   │   └── roles.yaml              # Defines IAM roles
  │   ├── loadbalancer                # Load balancer-related resources
  │   │   ├── alb.yaml                # Defines the Application Load Balancer (ALB)
  │   │   └── nlb.yaml                # Defines the Network Load Balancer (NLB)
  │   ├── networking                  # Network-related resources
  │   │   ├── security-group.yaml     # Defines security groups
  │   │   ├── subnets.yaml            # Defines subnets
  │   │   └── vpc.yaml                # Defines the VPC
  │   ├── storage                     # Storage-related resources (S3, EFS, etc.)
  │   └── README.md                   # Project documentation
  └── .gitignore                      # Git ignore rules

```

## References

- [[Github] aws-cloudformation-fargate](https://github.com/nathanpeck/aws-cloudformation-fargate)