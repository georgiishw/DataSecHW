(this document has been falsely submitted under h2, resulting in it being inaccessible by peer reviewers, i have informed the teacher by email as soon as i realized my mistake)

h2

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

    The Cloud Hopper attack highlights the failure of several important security controls and emphasizes the need for a new security strategy in which organizations design their environments with the ability to quickly detect breaches and lessen their effects. The most sensible approach to security is one that bases everything on the principle of least privilege from the ground up, or what is known as a "Zero Trust" approach. This is because of how sophisticated attackers operate.

