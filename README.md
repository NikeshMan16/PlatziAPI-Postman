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
```

Install Newman report:

```bash
npm install -g newman-reporter
```

### Running the tests from command line using newman
```bash
newman run collections/Test-project-api.postman_collection.json
```


### Running the tests and report generation using newman CLI
1. Go to the project root directory
2. Open command prompt
3. Enter the following script
   ```bash
   newman run collections/Test-project-api.postman_collection.json -r html --reporter-html-export Report.html
   ```
4. Report.html is the html-report generated in the project root directory.

