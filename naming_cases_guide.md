# Complete Guide to Programming Naming Cases

## 1. camelCase

**Format:** First word lowercase, subsequent words capitalized
**Example:** `userName`, `calculateTotalPrice`, `isValidEmail`

**Primary Usage:**

- **JavaScript/TypeScript:** Variables, functions, methods, properties
- **Java:** Variables, methods, fields
- **C#:** Variables, fields, parameters, local methods
- **Swift:** Variables, functions, properties
- **Objective-C:** Methods, variables

## 2. PascalCase (UpperCamelCase)

**Format:** Every word starts with a capital letter
**Example:** `UserName`, `CalculateTotalPrice`, `IsValidEmail`

**Primary Usage:**

- **C#:** Classes, methods, properties, enums, namespaces
- **Java:** Classes, interfaces, enums
- **Pascal:** All identifiers (hence the name)
- **Swift:** Types, protocols, enums
- **JavaScript:** Constructor functions, classes
- **VB.NET:** Classes, methods, properties

## 3. snake_case

**Format:** All lowercase with underscores between words
**Example:** `user_name`, `calculate_total_price`, `is_valid_email`

**Primary Usage:**

- **Python:** Variables, functions, modules, packages
- **Ruby:** Variables, methods, symbols
- **C:** Variables, functions (traditional style)
- **Rust:** Variables, functions, modules
- **PHP:** Variables, functions (common style)
- **Database:** Column names, table names
- **Linux/Unix:** File names, directory names

## 4. SCREAMING_SNAKE_CASE (CONSTANT_CASE)

**Format:** All uppercase with underscores between words
**Example:** `MAX_USER_COUNT`, `DEFAULT_TIMEOUT_MS`, `API_BASE_URL`

**Primary Usage:**

- **Most languages:** Constants, environment variables
- **C/C++:** Preprocessor macros, constants
- **Java:** Static final constants
- **Python:** Module-level constants
- **JavaScript:** Constants
- **Configuration files:** Environment variables

## 5. kebab-case (dash-case, lisp-case)

**Format:** All lowercase with hyphens between words
**Example:** `user-name`, `calculate-total-price`, `is-valid-email`

**Primary Usage:**

- **CSS:** Class names, IDs, custom properties
- **HTML:** Attributes, data attributes
- **URLs:** Path segments, query parameters
- **Lisp/Clojure:** Functions, variables
- **Command line:** Flag names, file names
- **Docker:** Container names, image tags
- **Kubernetes:** Resource names

## 6. Train-Case (HTTP-Header-Case)

**Format:** Each word capitalized with hyphens between words
**Example:** `User-Name`, `Content-Type`, `Cache-Control`

**Primary Usage:**

- **HTTP:** Header names
- **MIME types:** Some parameter names
- **Some APIs:** Header conventions

## 7. dot.case

**Format:** Lowercase with dots between words
**Example:** `user.name`, `config.database.host`, `app.version`

**Primary Usage:**

- **Configuration files:** Property keys (Java properties, .env files)
- **Package names:** Reverse domain notation (Java packages)
- **Namespaces:** Some systems use dot notation
- **File extensions:** Multiple extensions like `.tar.gz`

## 8. flatcase

**Format:** All lowercase, no separators
**Example:** `username`, `calculatetotalprice`, `isvalidemail`

**Primary Usage:**

- **Domain names:** Cannot contain underscores or spaces
- **Some older systems:** Legacy naming conventions
- **Package names:** Some package managers (npm allows this)
- **Hashtags:** Social media tags

## 9. UPPERFLATCASE

**Format:** All uppercase, no separators
**Example:** `USERNAME`, `CALCULATETOTALPRICE`, `ISVALIDEMAIL`

**Primary Usage:**

- **Legacy systems:** Some old database systems
- **Assembly language:** Labels, constants
- **Some configuration:** Environment variable names (less common)

## 10. Hungarian Notation

**Format:** Type prefix + PascalCase or camelCase
**Example:** `strUserName`, `intCount`, `boolIsValid`, `objDatabase`

**Primary Usage:**

- **Legacy C/C++:** Variable naming (largely deprecated)
- **Visual Basic:** Traditional style (less common now)
- **Some embedded systems:** Type safety in C
- **Legacy Windows API:** Function and variable names

## 11. Reverse Hungarian (Apps Hungarian)

**Format:** Purpose prefix + PascalCase or camelCase
**Example:** `txtUserName`, `btnSubmit`, `lblError`, `chkRememberMe`

**Primary Usage:**

- **GUI frameworks:** Control naming (WinForms, VB6)
- **Visual Basic:** Form controls
- **Some web frameworks:** Element identification

## Quick Reference by Context

### Web Development

- **CSS:** kebab-case for classes, IDs
- **HTML:** kebab-case for attributes
- **JavaScript:** camelCase for variables/functions, PascalCase for classes
- **URLs:** kebab-case for paths

### Databases

- **Table names:** snake_case or PascalCase
- **Column names:** snake_case
- **Stored procedures:** varies by database

### Configuration

- **Environment variables:** SCREAMING_SNAKE_CASE
- **Config files:** dot.case or snake_case
- **Command line flags:** kebab-case

### File Systems

- **Linux/Unix:** snake_case or kebab-case
- **Windows:** PascalCase or camelCase (case-insensitive)
- **URLs/URIs:** kebab-case

## Best Practices

1. **Be consistent** within your project and team
2. **Follow language conventions** - don't fight the ecosystem
3. **Consider your audience** - APIs should follow expected patterns
4. **Use meaningful names** regardless of case style
5. **Avoid mixing cases** unless there's a specific technical reason
6. **Document your conventions** for team projects

## Language-Specific Recommendations

- **JavaScript/TypeScript:** camelCase (variables/functions), PascalCase (classes)
- **Python:** snake_case (everything except classes use PascalCase)
- **Java:** camelCase (variables/methods), PascalCase (classes)
- **C#:** PascalCase (public members), camelCase (private fields)
- **Go:** PascalCase (exported), camelCase (unexported)
- **Rust:** snake_case (variables/functions), PascalCase (types)
- **CSS:** kebab-case (classes/IDs)
- **Database:** snake_case (widely adopted standard)
