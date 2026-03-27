# API Specification

<!-- This file will be populated by Copilot based on PLAN.md requirements -->

## Base URL
`https://api.example.com/v1`

## Authentication
_Describe the authentication method._

## Endpoints

### Example Endpoint

| Method | Path | Description |
|--------|------|-------------|
| GET | `/resources` | List all resources |
| POST | `/resources` | Create a resource |
| GET | `/resources/:id` | Get a resource |
| PUT | `/resources/:id` | Update a resource |
| DELETE | `/resources/:id` | Delete a resource |

### Request/Response Examples

#### GET /resources
```json
{
  "data": [],
  "pagination": {
    "page": 1,
    "limit": 20,
    "total": 0
  }
}
```

## Error Codes
| Code | Description |
|------|-------------|
| 400 | Bad Request |
| 401 | Unauthorized |
| 404 | Not Found |
| 500 | Internal Server Error |
