# CYBR-8420 Requirements for Software Security Engineering

## Use Case Diagrams
### Misuse Case 1 - Augusto
![AugustoDiagram](https://github.com/user-attachments/assets/ec84fae2-5400-4e60-b7a4-fa45550d0d6f)
**Use Case**

An administrator is trying to update the source code to fix some minor issues.

**Misuse Case**

A malicious contributor modifies the code in the hopes that the administrator updates the program with their code, for the intent of stealing administrators log in credentials or creating new vulnerabilities so the threat actor can modify student grades.

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

While working on my Misuse Case, I initially created a chart that resembled more of a spaghetti dinner. I had way too many circles, prompts, solutions, and lines going everywhere. It was hard for me to pinpoint what I needed to do and clear the mess so it wasn’t impossible to read. After using a few prompts on ChatGPT, I was able to eliminate a lot of the issues I had and ended up with a clearer diagram. Some of my prompts were:

### **Prompt**  
Pretend you are a senior developer working on open-source software. Give me 5 issues that a malicious contributor can create and 5 solutions.

### **Answer**  
As a senior developer working on an open-source software project, here are five issues that a malicious contributor could introduce, along with five solutions to mitigate these risks:

### **Issues a Malicious Contributor Can Create:**

1. **Backdoor Implementation**  
   A malicious contributor might add hidden backdoors into the code, allowing unauthorized access to the system.

2. **SQL Injection Vulnerabilities**  
   They could introduce insecure code that is vulnerable to SQL injection attacks, compromising the application's database.

3. **Credential Theft**  
   The contributor may modify code to collect and exfiltrate sensitive information, such as admin passwords or tokens, to an external server.

4. **Malicious Dependencies**  
   They might introduce or modify dependencies that include malware or have known vulnerabilities, compromising the security of the entire application.

5. **Denial of Service (DoS) Mechanisms**  
   A contributor could insert code that triggers a resource exhaustion or infinite loop, leading to performance issues or system crashes, causing a denial of service.

### **Solutions to Mitigate These Issues:**

1. **Code Review and Approval Process**  
   Enforce strict peer-review processes for every contribution. Ensure that multiple trusted developers review and approve code changes before they are merged into the main project.

2. **Automated Static Code Analysis**  
   Use automated tools (e.g., SonarQube, Checkmarx) to scan code for vulnerabilities such as backdoors, SQL injection risks, and other security flaws before accepting contributions.

3. **Dependency Scanning Tools**  
   Implement automated tools (like Dependabot, Snyk) to scan for vulnerabilities in third-party dependencies and ensure only safe libraries are used in the project.

4. **Penetration Testing and Security Audits**  
   Conduct regular penetration tests and security audits on the project, especially after significant changes. Use tools like OWASP ZAP or Burp Suite to identify potential vulnerabilities.

5. **Digital Signature Verification for Contributions**  
   Use digital signatures for all commits to ensure that code is coming from a trusted contributor. Additionally, restrict merge privileges to a small group of trusted maintainers who review all contributions.


By implementing these safeguards, you can significantly reduce the risk of malicious contributions compromising the security of an open-source project.

---

## List of Security Requirements derived from misuse case analysis

 - Input Validation- Implement strict input validation to defend against SQL injection attacks using JavaScript or HTML5 to manage input validation parameters.
 - Access Control- Utilize session timeouts and CAPTCHA as means of access control. Session timeouts log a user out after a predetermined duration of inactivity. CAPTCHA requires text-based, image-based, or audio verification to prevent unauthorized access.

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


