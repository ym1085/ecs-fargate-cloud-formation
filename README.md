# ECS Fargate CloudFormation Template Sample

> Sample to conduct cloudformation test

## Package Structure

```bash
project-root/
├── cfn-templates/                               # Cloudformation Template 파일 위치
│   ├── master-template.yml                      # 마스터 템플릿 (Nested Stack)
│   ├── network.yml                              # VPC 및 네트워크 리소스
│   ├── iam.yml                                  # IAM 역할 및 정책
│   ├── ecs-cluster.yml                          # ECS 클러스터 정의
│   ├── task-definition.yml                      # 태스크 정의
│   ├── ecs-service.yml                          # ECS 서비스 정의
│   └── load-balancer.yml                        # 로드 밸런서 리소스
├── scripts/
│   ├── deploy.sh                                # 배포 스크립트
│   └── delete.sh                                # 리소스 삭제 스크립트
├── README.md
└── .gitignore
```

## References

- [[Github] aws-cloudformation-fargate](https://github.com/nathanpeck/aws-cloudformation-fargate)
- [[AWS] AWS Cloudformation으로 인프라 구축하기#1 – Network 구성하기](https://blog.bespinglobal.com/post/aws-cloudformation%EC%9C%BC%EB%A1%9C-%EC%9D%B8%ED%94%84%EB%9D%BC-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B01-network-%EA%B5%AC%EC%84%B1%ED%95%98%EA%B8%B0/)