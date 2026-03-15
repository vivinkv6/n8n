# N8N Development Setup

## Quick Start
 
1. **Start the services:**
   ```bash
   docker-compose up -d
   ```

2. **Access n8n:**
   - URL: http://localhost:5678
   - No authentication required (development mode)

## Key Features

- **Persistent Data**: All workflows and data are saved in Docker volumes
- **Auto-restart**: Services automatically restart if Docker is restarted
- **Simple Setup**: No SSL, no complex configuration needed
- **Development Focused**: Optimized for testing and development

## Data Persistence

Your data is stored in Docker volumes:
- `n8n_data`: n8n workflows, credentials, and settings
- `postgres_data`: Database storage

Even if you stop and restart Docker, your data will persist.

## Useful Commands

```bash
# Start services
docker-compose up -d

# Stop services
docker-compose down

# View logs
docker-compose logs n8n

# Check service status
docker-compose ps

# Remove everything (including data - USE WITH CARE)
docker-compose down -v
```
