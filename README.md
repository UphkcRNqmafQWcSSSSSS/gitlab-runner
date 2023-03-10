# 目录结构
```
├── README.md
├── .env.sample                 环境配置示例文件
├── gitlab.sample.rb            
└── docker-compose.sample.yml   Docker 服务配置示例文件
```

# GitLab Runner
```base
# 注册 runner
gitlab-runner register \
    --url https://gitlab.com/ \
    --registration-token Token \
    --tag-list "web" \
    --executor "docker" \
    --docker-image "alpine:latest" \
    --description "前端部署runner"
    
# 注销 runner
gitlab-runner unregister --name xxx
```