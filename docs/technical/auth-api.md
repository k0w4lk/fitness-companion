# Authentication API

## Registration
`POST /api/auth/register`

### Request
```json
{
  "email": "user@example.com",
  "password": "SecurePass123",
  "role": "client" | "trainer",
  
  // Optional trainer fields
  "trainer_profile": {
    "certifications": ["url1", "url2"],
    "specializations": ["yoga", "crossfit"]
  },
  
  // Optional client fields
  "client_profile": {
    "goals": ["weight_loss"],
    "preferences": ["group_classes"]
  }
}
```

### Responses

#### 201 Created
```json
{
  "id": "user_123",
  "email": "user@example.com",
  "role": "trainer",
  "profile_complete": false
}
```

#### 400 Bad Request
```json
{
  "error": "VALIDATION_ERROR",
  "details": {
    "email": "Already registered"
  }
}
```