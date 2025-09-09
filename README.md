# Jenkins Configuration as Code (JCasC)

A complete Jenkins setup using Configuration as Code approach for automated, reproducible CI/CD environments.

## Why JCasC?

Traditional Jenkins setup requires manual configuration through the web UI, making it:
- **Error-prone** - Manual clicks can lead to inconsistencies
- **Hard to replicate** - Difficult to recreate the same setup across environments
- **Not version-controlled** - Configuration changes aren't tracked

## Benefits

✅ **Automated Setup** - Zero manual configuration required  
✅ **Version Control** - All configurations tracked in Git  
✅ **Reproducible** - Identical environments every time  
✅ **Fast Deployment** - Complete Jenkins instance in minutes  
✅ **Team Collaboration** - Share configurations easily  
✅ **Disaster Recovery** - Quick restoration from code  

## Quick Start

```bash
# Clone and start Jenkins
git clone <repository-url>
cd JCasC
docker-compose up -d

# Access Jenkins at http://localhost:8080
# Login: admin/admin123
```

## What's Included

- **Pre-configured Users** - Admin, developer, and viewer roles
- **Essential Plugins** - Git, Pipeline, Docker, BlueOcean, and more
- **Build Tools** - Maven, Gradle, Node.js, Docker pre-installed
- **Security** - Proper authentication and authorization
- **Credentials** - GitHub, SSH, and API token templates

## Configuration Files

- `jenkins.yaml` - Main JCasC configuration
- `plugins.txt` - Required Jenkins plugins
- `docker-compose.yml` - Container orchestration
- `Dockerfile` - Custom Jenkins image

## Customization

Edit `jenkins.yaml` to modify:
- User accounts and permissions
- Plugin configurations
- Build tools and versions
- Global settings and credentials

Changes apply automatically on container restart.