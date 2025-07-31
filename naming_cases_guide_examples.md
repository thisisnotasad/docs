# Complete Guide to Programming Naming Cases

## 1. camelCase

**Format:** First word lowercase, subsequent words capitalized
**Example:** `userName`, `calculateTotalPrice`, `isValidEmail`

**Most Common Usage: JavaScript**

```javascript
const userName = "john_doe";
const totalPrice = 99.99;

function calculateTotalPrice(items) {
  return items.reduce((sum, item) => sum + item.price, 0);
}

const userProfile = {
  firstName: "John",
  lastName: "Doe",
  isActive: true,
};
```

## 2. PascalCase (UpperCamelCase)

**Format:** Every word starts with a capital letter
**Example:** `UserName`, `CalculateTotalPrice`, `IsValidEmail`

**Most Common Usage: C# Classes**

```csharp
public class UserManager {
    public string UserName { get; set; }
    public enum UserStatus { Active, Inactive, Pending }

    public bool ValidateUserCredentials(string username, string password) {
        return true;
    }
}
```

## 3. snake_case

**Format:** All lowercase with underscores between words
**Example:** `user_name`, `calculate_total_price`, `is_valid_email`

**Most Common Usage: Python**

```python
user_name = "john_doe"
max_retry_count = 3

def calculate_total_price(items):
    total_sum = 0
    for item in items:
        total_sum += item.price
    return total_sum

class UserManager:
    def __init__(self, database_url):
        self.database_url = database_url

    def is_valid_email(self, email_address):
        return "@" in email_address
```

## 4. SCREAMING_SNAKE_CASE (CONSTANT_CASE)

**Format:** All uppercase with underscores between words
**Example:** `MAX_USER_COUNT`, `DEFAULT_TIMEOUT_MS`, `API_BASE_URL`

**Most Common Usage: Constants (All Languages)**

```javascript
const MAX_RETRY_ATTEMPTS = 3;
const API_BASE_URL = "https://api.example.com";
const DEFAULT_TIMEOUT_MS = 5000;

function fetchUserData(userId) {
  return fetch(`${API_BASE_URL}/users/${userId}`, {
    timeout: DEFAULT_TIMEOUT_MS,
  });
}
```

## 5. kebab-case (dash-case, lisp-case)

**Format:** All lowercase with hyphens between words
**Example:** `user-name`, `calculate-total-price`, `is-valid-email`

**Most Common Usage: CSS**

```css
.user-profile-card {
  background-color: #f5f5f5;
  border-radius: 8px;
}

.nav-menu-item {
  padding: 10px 15px;
  margin-bottom: 5px;
}

#main-content-area {
  max-width: 1200px;
  margin: 0 auto;
}

:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --border-radius-default: 4px;
}
```

## 6. Train-Case (HTTP-Header-Case)

**Format:** Each word capitalized with hyphens between words
**Example:** `User-Name`, `Content-Type`, `Cache-Control`

**Most Common Usage: HTTP Headers**

```http
GET /api/users HTTP/1.1
Host: api.example.com
Content-Type: application/json
Accept: application/json
User-Agent: MyApp/1.0
Cache-Control: no-cache
Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9
X-Request-ID: 12345-67890-abcdef
X-Rate-Limit-Remaining: 100
```

## 7. dot.case

**Format:** Lowercase with dots between words
**Example:** `user.name`, `config.database.host`, `app.version`

**Most Common Usage: Java Properties**

```properties
app.name=MyApplication
app.version=1.2.0
database.host=localhost
database.port=5432
database.name=myapp_db
server.port=8080
logging.level.root=INFO
security.jwt.secret=mySecretKey
cache.expiry.minutes=60
```

## 8. flatcase

**Format:** All lowercase, no separators
**Example:** `username`, `calculatetotalprice`, `isvalidemail`

**Most Common Usage: Domain Names**

```
example.com
mycompanyname.org
userprofileservice.net
socialmediaplatform.io
```

## 9. UPPERFLATCASE

**Format:** All uppercase, no separators
**Example:** `USERNAME`, `CALCULATETOTALPRICE`, `ISVALIDEMAIL`

**Most Common Usage: Assembly Language**

```assembly
.DATA
USERNAME    DB 'admin', 0
MAXRETRIES  EQU 3
BUFFERSIZE  EQU 1024

.CODE
MAIN PROC
    MOV AX, MAXRETRIES
    CALL VALIDATEUSER
    JMP EXITPROGRAM
MAIN ENDP

VALIDATEUSER PROC
    RET
VALIDATEUSER ENDP
```

## 10. Hungarian Notation

**Format:** Type prefix + PascalCase or camelCase
**Example:** `strUserName`, `intCount`, `boolIsValid`, `objDatabase`

**Most Common Usage: Legacy C/C++**

```cpp
int intUserCount = 0;
char* strUserName = "john_doe";
bool boolIsActive = true;
float fltTotalPrice = 99.99f;

struct UserProfile {
    int intUserId;
    char strFirstName[50];
    char strLastName[50];
    bool boolIsVerified;
};

void ProcessUserData(int intUserId, char* strUserName, bool boolSendEmail) {
    if (boolSendEmail && strUserName != NULL) {
        SendNotification(strUserName);
    }
}
```

## 11. Reverse Hungarian (Apps Hungarian)

**Format:** Purpose prefix + PascalCase or camelCase
**Example:** `txtUserName`, `btnSubmit`, `lblError`, `chkRememberMe`

**Most Common Usage: Windows Forms**

```csharp
public partial class LoginForm : Form {
    private TextBox txtUsername;
    private TextBox txtPassword;
    private Button btnLogin;
    private Button btnCancel;
    private Label lblError;
    private CheckBox chkRememberMe;

    private void btnLogin_Click(object sender, EventArgs e) {
        if (string.IsNullOrEmpty(txtUsername.Text)) {
            lblError.Text = "Please enter username";
            lblError.Visible = true;
            return;
        }

        bool rememberUser = chkRememberMe.Checked;
        ValidateCredentials(txtUsername.Text, txtPassword.Text);
    }
}
```

## Quick Reference Summary

| Case                 | Primary Usage                  | Example        |
| -------------------- | ------------------------------ | -------------- |
| camelCase            | JavaScript variables/functions | `userName`     |
| PascalCase           | C# classes, Java classes       | `UserManager`  |
| snake_case           | Python everything              | `user_name`    |
| SCREAMING_SNAKE_CASE | Constants everywhere           | `MAX_COUNT`    |
| kebab-case           | CSS classes/IDs                | `user-profile` |
| Train-Case           | HTTP headers                   | `Content-Type` |
| dot.case             | Java properties                | `app.name`     |
| flatcase             | Domain names                   | `example.com`  |
| UPPERFLATCASE        | Assembly language              | `USERNAME`     |
| Hungarian            | Legacy C/C++                   | `strUserName`  |
| Reverse Hungarian    | GUI controls                   | `txtUsername`  |

## Best Practices

1. **Follow language conventions** - Each language has established patterns
2. **Be consistent** within your project
3. **Consider your context** - Web, desktop, mobile, etc.
4. **Think about your team** - Use what everyone understands
5. **Avoid mixing cases** unless technically required
