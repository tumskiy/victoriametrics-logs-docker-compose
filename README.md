# VictoriaLogs with Grafana Docker Stack
## Quick Start

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/victorialogs-grafana.git
   cd victorialogs-grafana
   ```
2. Start the services:

```bash
docker compose up -d
```
3. Access the services:
```
Grafana: http://localhost:3000 (admin/admin)
```
```
VictoriaLogs API: http://localhost:9428
```
ENV
```yaml
 environment:
      - GF_SECURITY_ADMIN_USER=admin
      - GF_SECURITY_ADMIN_PASSWORD=admin
```

## Setting Up Grafana

Log in to Grafana at http://localhost:3000

Navigate to "Connections" → "Data sources"

The VictoriaLogs datasource should be pre-configured at `http://victorialogs:9428`

Verify connection with "Save & test" button
