---
title: API Name
date: YYYY-MM-DD
category: api
tags: [api, endpoint, rest]
---

# API Name

Brief description of what this API does.

이 API가 수행하는 작업에 대한 간략한 설명.

## Endpoint

```
{HTTP_METHOD} /api/v1/endpoint-path
```

## Authentication

Required authentication method.

필요한 인증 방법.

```
Authorization: Bearer {token}
```

## Request

### Headers

| Header | Type | Required | Description |
|--------|------|----------|-------------|
| Content-Type | string | Yes | application/json |
| Authorization | string | Yes | Bearer token |

### Parameters

#### Path Parameters

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| id | string | Yes | Resource identifier |

#### Query Parameters

| Parameter | Type | Required | Default | Description |
|-----------|------|----------|---------|-------------|
| page | integer | No | 1 | Page number |
| limit | integer | No | 10 | Items per page |

### Request Body

```json
{
  "field1": "value1",
  "field2": "value2",
  "field3": {
    "nested_field": "nested_value"
  }
}
```

#### Request Schema

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| field1 | string | Yes | Description of field1 |
| field2 | string | No | Description of field2 |
| field3 | object | No | Description of field3 |

## Response

### Success Response

**Status Code**: `200 OK`

```json
{
  "status": "success",
  "data": {
    "id": "123",
    "field1": "value1",
    "field2": "value2"
  }
}
```

#### Response Schema

| Field | Type | Description |
|-------|------|-------------|
| status | string | Response status |
| data | object | Response data |
| data.id | string | Resource ID |
| data.field1 | string | Field 1 value |
| data.field2 | string | Field 2 value |

### Error Responses

#### 400 Bad Request

```json
{
  "status": "error",
  "error": {
    "code": "INVALID_REQUEST",
    "message": "Invalid request parameters"
  }
}
```

#### 401 Unauthorized

```json
{
  "status": "error",
  "error": {
    "code": "UNAUTHORIZED",
    "message": "Authentication required"
  }
}
```

#### 404 Not Found

```json
{
  "status": "error",
  "error": {
    "code": "NOT_FOUND",
    "message": "Resource not found"
  }
}
```

#### 500 Internal Server Error

```json
{
  "status": "error",
  "error": {
    "code": "INTERNAL_ERROR",
    "message": "An unexpected error occurred"
  }
}
```

## Examples

### Example 1: Basic Request

```bash
curl -X {HTTP_METHOD} https://api.example.com/api/v1/endpoint-path \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -d '{
    "field1": "value1",
    "field2": "value2"
  }'
```

### Example 2: Using Query Parameters

```bash
curl -X GET https://api.example.com/api/v1/endpoint-path?page=1&limit=20 \
  -H "Authorization: Bearer YOUR_TOKEN"
```

## Rate Limiting

Rate limiting information for this API.

이 API의 속도 제한 정보.

- Rate limit: 100 requests per minute
- Header: `X-RateLimit-Remaining`

## Notes

Additional notes and considerations.

추가 참고 사항 및 고려 사항.

- Note 1
- Note 2

## Related Endpoints

- [Related API 1](./related-api-1.md)
- [Related API 2](./related-api-2.md)

---

**Last Updated**: YYYY-MM-DD
