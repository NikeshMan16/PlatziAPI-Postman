# Postman API Test Collection 

This repository contains automated API tests using [Postman](https://www.postman.com/) and [Newman](https://www.npmjs.com/package/newman), Postman's command-line tool.

## File Structure

- `collections/`: Contains exported Postman test collections (v2.1).
- `environments/`: (Optional) Postman environments for different environments like `dev`, `staging`, etc.
- `.github/workflows/`: Contains the GitHub Actions workflow to run Newman tests on every push.

## ▶️ Running Tests Locally with Newman

### Prerequisite

Install Newman:

```bash
npm install -g newman
