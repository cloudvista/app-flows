### Issue Capture Template


| Issue | Text |
| -- | -- |
| Description | Short description|
| Actual | Actual behaviour |
| Expected | Expected or desired behaviour|
| Reproduce | Steps to reproduce |


Example: Login Button Unresponsive

__Description__  
The login button becomes unresponsive after three failed login attempts.

__Steps to Reproduce__  
1. Navigate to the login page  
2. Enter incorrect credentials three times  
3. Observe that the login button no longer responds to clicks  

__Expected Behavior__  
The login button should remain clickable, displaying an error message for too many attempts.

__Actual Behavior__  
The login button becomes grayed out and unresponsive.

__Error Flow Diagram__  
```mermaid
flowchart TD
    A[User on Login Page] --> B{Enter Credentials}
    B -->|Incorrect| C[Failed Attempt]
    C --> D{Attempt Count < 3?}
    D -->|Yes| B
    D -->|No| E[Login Button Unresponsive]
    B -->|Correct| F[Successful Login]
