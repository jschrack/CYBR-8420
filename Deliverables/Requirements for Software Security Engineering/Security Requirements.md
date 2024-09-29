# CYBR-8420 Requirements for Software Security Engineering

## Use Case Diagrams
### Interaction 1 - Augusto
### Misuse Case 2 - Student updates gradebook
![Misuse Case 2 - Instrutor udpates gradebook](https://github.com/jschrack/CYBR-8420/blob/peachykeen00-patch-1/Deliverables/Requirements%20for%20Software%20Security%20Engineering/Misuse-Case2.png)

**Use Case**

An instructor logs into the gradebook system to update students' grades.

**Misuse Case**

An unauthorized student gains access to the gradebook system with an objective to manipulate the gradebook, either by altering their own grades or those of their peers by using Session Hijacking, Cross-Site Request Forgery (CSRF), or SQL injection.


### Interaction 3 - Geoff
### Interaction 4 - Jesse
### Interaction 5 - Mark

## AI Prompt

## List of Security Requirements derived from misuse case analysis

 - Input Validation- Implement strict input validation to defend against SQL injection attacks using JavaScript or HTML5 to manage input validation parameters.
 - Access Control- Utilize session timeouts and CAPTCHA as means of access control. Session timeouts log a user out after a predetermined duration of inactivity. CAPTCHA requires text-based, image-based, or audio verification to prevent unauthorized access.
-	Automated Static Code Analysis - Implement tools that automatically analyze the codebase for potential vulnerabilities and suspicious changes to catch issues early.
-	Penetration Testing / Security Audits - Regularly conduct penetration tests or security audits to identify vulnerabilities that may have been introduced, using tools like OWASP ZAP to find injection flaws or other weaknesses.
-	Trusted Contributor Programs - Limit write access to trusted contributors or maintainers and use digital signatures for contributions to ensure code authenticity.

## Security Requirements Assesment

Canvas LMS advertises the following security features that mitigate security requirements derived from the misuse case analyses.

 - Input Validation:
   - CSRF Protection / Cross-Site Scripting (XSS) Protection
   - Audit Logs

 - Access Controls:
   - Session Timeouts
   - Role-Based Access Control (RBAC)

## Link to Project Board
[Click here to view the board](https://github.com/users/jschrack/projects/2/views/1)

## Individual Contribution Summaries
### Augusto
### Deb

- Completed misuse case analysis for the instructor / gradebook relationship
- Built list of security requirements dervied from misuse case analysis and compared them to advertised security features of software to determine sufficiency of current security features
- Researched OSS security configuration / installation documentation for Canvas LMS and contributed this section in Part II of the assignment
  
### Geoff
### Jesse
### Mark
## Team Reflection


