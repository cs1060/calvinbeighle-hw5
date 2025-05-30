# Homework 5: SQL Injection and Penetration Testing

## 5.1: Linear Setup
- Accepted the email invitation and joined the project team
- Reviewed the Start Guide from the Linear documentation
- Created two Linear tasks with "HW5" labels for completing sections 5.2 and 5.3

## 5.2: SQL Injection Attack
Created a test.json file with initial data:
```json
{"zip":"84601","measure_name":"Adult obesity"}
```

Used it to test the endpoint:
```bash
curl -X POST https://cat-hw4.vercel.app/county_data -H "Content-Type: application/json" -d @test.json
```

### Models Used for SQL Injection Attack
Used Claude 3 Sonnet through the Cursor IDE to develop and test SQL injection attacks. The model helped identify potential vulnerabilities and develop effective injection strategies while working within ethical boundaries.

## 5.3: Vulnerability Scanner
Built a Python program using Claude 3 Sonnet in Cursor that:
- Scans open TCP ports on localhost using nmap
- Tests HTTP and SSH connections with a dictionary of credentials
- Reports successful connections in RFC 3986 syntax

The program handles exceptions gracefully and can be run with a -v option for verbose output. 