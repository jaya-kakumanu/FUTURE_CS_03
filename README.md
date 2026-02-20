# 📘 API Security Risk Analysis – FUTURE_CS_03

## 🎯 Objective
The objective of this task is to perform a read-only API security assessment on a public demo API to identify common API security risks such as unauthenticated access, excessive data exposure, and missing security controls.

---

## 🔎 API Selected
**JSONPlaceholder (Public Test API)**  
https://jsonplaceholder.typicode.com

This API was chosen because it is publicly available, safe for testing, and contains only demo data.

---

## 🛠 Tools Used
- Postman (API testing)
- Web Browser (Documentation review)
- Kali Linux Terminal (Header inspection using curl)
- GitHub (Project documentation)

---

## 🧪 Endpoints Tested
- `/posts`
- `/users`
- `/comments`

---

## 🔍 Security Findings

### ⚠️ Unauthenticated Endpoints
All tested endpoints were accessible without authentication.

**Risk Level:** Medium

---

### ⚠️ Excessive Data Exposure
The users endpoint returns complete user objects including contact and address information.

**Risk Level:** Medium

---

### ⚠️ Missing Rate Limiting Indicators
No visible rate-limiting headers were observed.

**Risk Level:** Medium

---

### ⚠️ Public Demo Data
The API contains only sample data and no real sensitive information.

**Risk Level:** Low

---

## 🛡️ Recommendations
- Implement authentication tokens (API key or OAuth)
- Limit unnecessary fields in responses
- Enable rate limiting
- Apply proper input validation
- Use security headers

---

## 📂 Repository Structure
