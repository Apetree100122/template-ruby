# SQL Injection

## Overview

<!--
**Please replace text in each section below**

SQL Injection Vulnerability Report

Resources:

- <https://owasp.org/www-community/attacks/SQL_Injection>
- <https://owasp.org/www-community/attacks/Blind_SQL_Injection>
-->


SQL Injection is a vulnerability in which an application injects a valid payload within a SQL query from input data.

SQL queries may be exploited in a variety of ways including exfiltration of database data, exfiltration of files, subtle data tampering, and resource exhaustion. A common escalation is to abuse the SQL functionality to upgrade to full remote command execution.

A SQL Injection (SQLi) was discovered at {{target}} at {{url}} through {{parameter}} using {{payload}}. This allows a malicious attacker to {{action}} and perform arbitrary SQL queries.

## Walkthrough & PoC
<!--
Provide a step-by-step walkthrough on how to access the vulnerable injection point, and how to exploit the vulnerability.
Adding a dot-pointed walkthrough with relevant screenshots will speed triage time and result in faster rewards!
-->

1. Login to in-scope asset at {{url}}
2. Browse to account page
3. Modify ID token to add single quote
4. View error which states 'SQL Syntax Error'
5. Replace ID value with {{payload}}

## Vulnerability Evidence
<!--
Your submission MUST include evidence of the vulnerability and not be theoretical in nature.

For an SQL Injection vulnerability, please include specific NON-PII information discovered in the database, such as Database Version, a listing of database tables, or an injected 'sleep' payload.

You may present your evidence as output from a tool such as SQLMap, unless the program forbids the use of these tools, and it may be in the format of terminal output, screenshots, or video..

**DO NOT ACCESS PII**
-->

The screenshot/video below demonstrates the SQLi being executed at {{url}}.

{{screenshot}}

## Demonstrated Impact
<!--
Demonstrating access to data other than the database version or database tables is NOT permitted without explicit permission from the program.
**DO NOT ACCESS PII**
--> 

A malicious attacker could theoretically abuse this specific SQLi further to {{action}} by using the following SQL query:

```sql
{{payload}}
```
