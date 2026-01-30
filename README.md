# Ethical Considerations
Remember that hacking into devices without permission is illegal and unethical. 
Always ensure you have the necessary permissions and are conducting these activities in a 
controlled environment for educational or security assessment purposes.

# Topics
## SQL injections (SQLi)

<details>
<summary style="cursor:pointer">Loading from memory</summary>
Manuell detection
- The single quote character ' and look for errors or other anomalies.
- Some SQL-specific syntax that evaluates to the base (original) value of the entry point, and to a different value, and look for systematic differences in the application responses.
- Boolean conditions such as OR 1=1 and OR 1=2, and look for differences in the application's responses.
- Payloads designed to trigger time delays when executed within a SQL query, and look for differences in the time taken to respond.
- OAST payloads designed to trigger an out-of-band network interaction when executed within a SQL query, and monitor any resulting interactions.
  
Alternatively and automaticly use the Burp Scanner to find the majority of SQL injection vulnerabilities.

```bash
```
</details>
