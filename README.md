# 目录结构
```
├── README.md
├── .env.sample                 环境配置示例文件
├── gitlab.sample.rb            
└── docker-compose.sample.yml   Docker 服务配置示例文件
```

# GitLab
```base
# 重载配置
gitlab-ctl reconfigure

# 重启服务
gitlab-ctl restart

# 检查恢复状态
gitlab-rake gitlab:check SANITIZE=true
```

# GitLab Runner
```base
# 注册 runner
gitlab-runner register
```