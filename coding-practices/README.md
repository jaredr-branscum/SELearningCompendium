# General Coding Practices
https://code.tutsplus.com/tutorials/top-15-best-practices-for-writing-super-readable-code--net-8118

https://google.github.io/eng-practices/

# General Unit Testing
https://www.testim.io/blog/unit-testing-best-practices/

# Typescript
https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html

# Code Review Security Checklist
1 Input Validation
- Check if all incoming data is properly validated.
- Secure SQL? Always use parameterized queries—never concatenate strings.
- Frontend output? Escape everything to prevent XSS.

2 Authentication & Sessions
- Passwords? Make sure bcrypt or Argon2 is used for hashing.
- CSRF protected? Always include tokens in sensitive requests.
- Inactive sessions? Configure timeouts to prevent session hijacking.

3 Sensitive Data
- Are critical data encrypted (e.g., AES-256)?
- Is the code enforcing HTTPS everywhere?
- Logs or error messages? No exposing sensitive information.

4 Security Configuration
- Are file and directory permissions properly restricted?
- Debugging/testing disabled in production?
- Is Content Security Policy (CSP) being applied?

5 Dependencies
→ Check if libraries/frameworks are up to date.
→ Any tool like Dependabot configured to flag vulnerabilities?

6 Access Control
- Every sensitive route and function has proper permission checks?
- Principle of least privilege applied to roles and users?

