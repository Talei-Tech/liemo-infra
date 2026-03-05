# ⚙️ Liemo Infrastructure

> Infrastructure as Code for the Liemo platform — Terraform, Docker, CI/CD.

## Structure

```
liemo-infra/
├── terraform/
│   ├── modules/
│   │   ├── vpc/
│   │   ├── rds/
│   │   ├── ecs/
│   │   ├── s3/
│   │   └── cloudfront/
│   ├── environments/
│   │   ├── staging/
│   │   └── production/
├── docker/
│   ├── api/
│   ├── nginx/
│   └── docker-compose.yml
├── .github/
│   └── workflows/
│       ├── api-ci.yml
│       ├── mobile-ci.yml
│       ├── web-ci.yml
│       └── infra-plan.yml
```

## Prerequisites
- Terraform >= 1.6
- AWS CLI configured
- Docker Desktop

## Deploy

```bash
cd terraform/environments/staging
terraform init
terraform plan
terraform apply
```

---
*Liemo — Live Store Link Aggregator | Philippines 🇵🇭 & Kuwait 🇰🇼*
