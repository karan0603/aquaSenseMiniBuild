# AquaSense API Test Plan

| ID | Test Scenario | Expected Result |
|---|---|---|
| TC01 | Login with valid credentials | 200 OK and authentication token returned |
| TC02 | Login with invalid credentials | Login rejected with 401 Unauthorized |
| TC03 | Get device status with valid token | 200 OK with tank level, pump state and last_seen |
| TC04 | Access API with invalid token | 401 Unauthorized |
| TC05 | Access API without token | 401 Unauthorized |
| TC06 | Request status for unknown device ID | 404 Not Found |
| TC07 | Device is offline or last_seen is stale | App should indicate that device data may be outdated |
| TC08 | API returns missing or invalid fields | App should handle the response safely without crashing |

## Testing Notes

The positive login and device-status scenarios were tested using Postman Mock Server.

The remaining scenarios are documented test cases but were not executed against a real backend because no live API was provided.
