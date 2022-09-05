(this document has been falsely submitted under h2, resulting in it being inaccessible by peer reviewers, i have informed the teacher by email as soon as i realized my mistake)

h2

x) read and sum

OWASP Top 10 (2021)

Security Misconfiguration

    This entry is placed 5th in the OWASP Top 10 of 2021.

    It has been an emerging risk since modern software is becoming more and more configurable.

    Such software may have things like:

    Extra features enabled
    Built-in accounts, which are usually overlooked and unchanged
    Error handlers and error messages that might expose unnecessary information to the user.

    To help prevent such vulnerabilities from happening, it is important to have repeatable hardening processes that ensure the identical and possibly automated configuration of secure environments for each individual system.

Vulnerable and Outdated Components

    This entry is placed 6th in the OWASP Top 10 of 2021.

    There is a higher chance of being vulnerable if you are using older software that has not been updated regularly, or if the software is out of date or unsupported. A lack of keeping up with new information can also mean you are at risk of having to upgrade your software more frequently.

Injection

    This entry is placed 3rd in the OWASP Top 10 of 2021.

    This is a technique used for modifying or retrieving data from SQL databases by sending statements that have not been validated, filtered, or sanitized by the server or application.

    In order to prevent this attack the data should be kept separately from commands and queries, and automated testing of all parameters, headers, URL, cookies, JSON, SOAP, and XML data inputs should be carried out by using server-side input validation, APIs that do not use interpreters, restricting the amount of data that can be requested, or other similar measures.

Cloud Hopper

    The Cloud Hopper attack highlights the failure of several important security controls and emphasizes the need for a new security strategy in which organizations design their environments with the ability to quickly detect breaches and lessen their effects.
    The most sensible approach to security is one that bases everything on the principle of least privilege from the ground up, or what is known as a "Zero Trust" approach. This is because of how sophisticated attackers operate.

CVE-2014-6271

    Codenamed "Shellshock" or "Bash Bug", this vulnerability allowed an attacker to gain control over a targeted computer if exploited successfully.
            It affected most versions of the Linux and Unix operating systems, in addition to Mac OS X (which is based around Unix).
            While any computer running Bash could be impacted by the vulnerability, a remote attacker can only use it under specific conditions.
            An attacker must force an application to send a malicious environment variable to Bash for a successful attack to take place.
            A successful attack on a Web server that contains this vulnerability could have major consequences.
            Attackers might be able to download malware onto infected computers or dump password files, for instance.
            The attackers could compromise and infect other network computers after getting past the victim's firewall.
            
a) SQLZoo

0 SELECT basics

![image](https://user-images.githubusercontent.com/90117364/188502450-e9f75c21-c958-4824-861c-70024e497f04.png)

![image](https://user-images.githubusercontent.com/90117364/188502478-bcd7f750-94c5-455c-9715-37cddbe8e324.png)

![image](https://user-images.githubusercontent.com/90117364/188502519-7165c247-9de7-4282-a71b-4a3d6a3156af.png)

2 SELECT from World

![image](https://user-images.githubusercontent.com/90117364/188503007-a8827c09-2fee-43d8-845f-bc2de06efede.png)

![image](https://user-images.githubusercontent.com/90117364/188503022-8f031f59-2cf1-4252-8630-4ff058c1f7e8.png)

![image](https://user-images.githubusercontent.com/90117364/188503054-80071414-2afa-4a0c-aa69-eefc77ea5176.png)

![image](https://user-images.githubusercontent.com/90117364/188503069-e38f2650-def4-497b-a79c-38f88ee5670f.png)

![image](https://user-images.githubusercontent.com/90117364/188506857-c0e44a61-fc82-40e3-ba8c-3b3762ea3485.png)

![image](https://user-images.githubusercontent.com/90117364/188503133-69a17fad-6da8-4a25-9814-0434c6e42255.png)

![image](https://user-images.githubusercontent.com/90117364/188503152-76d4ed14-8f8b-4591-ae8b-11b24b7e4888.png)

![image](https://user-images.githubusercontent.com/90117364/188503185-6b208c95-ed45-49db-a318-6e62b9fe81d0.png)

![image](https://user-images.githubusercontent.com/90117364/188503204-575314e6-f3d3-45d0-a0fb-f7265b3bb3a1.png)

![image](https://user-images.githubusercontent.com/90117364/188503255-6dedfb99-101f-4e0f-b5c8-b37174a4af6a.png)

![image](https://user-images.githubusercontent.com/90117364/188503681-73dae42f-837e-43d6-9a18-bf72f433ef20.png)

( this one's not fully migrated to the new function format such as LENGTH() ->  LEN() )

![image](https://user-images.githubusercontent.com/90117364/188504029-b16ffb6a-32c3-473d-9c65-f36ce1011585.png)

![image](https://user-images.githubusercontent.com/90117364/188504082-dc92dbe5-05fb-4976-b287-b6a3f8b53e54.png)

b) WebGoat

A1 Injection

 task 2 SQL
 
 employee data retrieval:
 
    SELECT department FROM Employees WHERE first_name = 'Bob'
    
![image](https://user-images.githubusercontent.com/90117364/188506721-6635ed9b-5f23-4c71-ad34-86f5cddd2206.png)


task 3 Data Manipulation Language (DML)

changing employees department:

    UPDATE Employees SET department = 'Sales' WHERE first_name = 'Tobi' AND last_name = 'Barnett'
    
![image](https://user-images.githubusercontent.com/90117364/188504956-e813b590-cfa2-43cd-88df-23e9db5b0897.png)

task 4 Data Definition Language (DDL)

making changes to the table:

    ALTER TABLE Employees ADD phone VARCHAR(20)
    
![image](https://user-images.githubusercontent.com/90117364/188506682-f0f01482-eaa5-47ec-b30a-7362eeded861.png)

task 5 Data Control Language (DCL)

granting permission to modify the table:

    GRANT ALTER TABLE TO UnauthorizedUser
    
![image](https://user-images.githubusercontent.com/90117364/188505193-dc5e82a5-8b16-4c7c-bdba-2184041f0f4a.png)

task 9 String SQL injection

exploiting concatenated strings:

    ' OR '1' = '1

![image](https://user-images.githubusercontent.com/90117364/188506616-23fcd3c7-94f9-403b-89c7-a8284a825f45.png)

task 10 Numeric SQL injection

exploiting numbers in concatenated strings:

    Login_Count:1 (or any other number)
    User_Id: '123' OR '1' = '1'
    
![image](https://user-images.githubusercontent.com/90117364/188506006-97e331b1-4260-4bc8-8571-f4587a3cb9a3.png)

task 11 Compromising confidentiality with String SQL injection

compromising data by exploiting concatenated strings:

    Employee Name: ' OR 1=1 --
    TAN: 3SL99A
    
![image](https://user-images.githubusercontent.com/90117364/188506201-ca8d1a1f-930e-43d7-b9c3-5bcd4e382be5.png)

task 12 Compromising integrity with Query chaining

compromising data by exploiting concatenated strings in the query:

    Employee Name: '; UPDATE employees SET salary = 999999 WHERE userid = 37648
    TAN: 3SL99A
    
![image](https://user-images.githubusercontent.com/90117364/188506316-1b8365a8-c750-4956-aa98-28db5ffd36c6.png)

task 13 Compromising availability

modifying availability of data:

    '; DROP TABLE access_log; --
    
![image](https://user-images.githubusercontent.com/90117364/188506501-f43f0f64-1534-4afc-851a-9d37d8426b33.png)

