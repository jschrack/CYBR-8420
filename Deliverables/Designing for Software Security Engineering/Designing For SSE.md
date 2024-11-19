# CYBR-8420 Designing for Software Security Engineering

## Link to Project Board
[Click here to view the board](https://github.com/users/jschrack/projects/5/views/1)

---

## Data Flow Diagram

[Threat Modeling Report](https://jschrack.github.io/CYBR-8420/Deliverables/Designing%20for%20Software%20Security%20Engineering/threat_modeling_report.html)

![Assurance Case 1](./Diagrams/DFD.png)

## Part 2 Observations

After reviewing the threat modeling report, we concluded as a team that the following numbers need more investigation: #2, #9, #15

Canvas LMS is designed with security in mind, but like any software platform, it may still be susceptible to vulnerabilities. In some places, the documentation recommends that Canvas use a privileged account on the database server when even when admin privileges are not required. Also, while Canvas supports private key database server validation, there is no recommendation made for it in the documentation. Although the platform provides protections against CSRF and XSS attacks, this does not guarantee that its mitigation capabilities are entirely free of flaws or limitations.

Another potential designed ga could be elevation by changing the execution flow in web server. Canvas LMS has basic input validation but needs additional protection from program flow integrity. This could be done by implementing input validation on every input (updated with new vulnerability finds) and code integrity checks to prevent attackers from altering the web server’s execution flow.

Canvas LMS potentially lacks input validation within the codebase. Since there are numerous where validation would need to be verified, this issue still needs to be investigated. Where possible, sanitization should be performed with standardized and automated means such as taint analysis. One promising emerging approach is to verify sanitization checks with AI-based tools. In our manual source review, proper input validation and sanitization were in place.


## Team Reflection

This week’s assignment was a bit different from the previous ones in terms of dividing the workload and coordinating our inputs. In the last two assignments, each team member was responsible for creating a diagram. However, for this assignment, we quickly determined that only one diagram was needed. One teammate took on the task of creating and updating the diagram, while the rest of us divided up the threats. Afterward, we had to determine the best way to coordinate and compile our inputs, as GitHub didn’t seem practical for this purpose. Most of our coordination was done through Discord via chat and voice discussions. We used a Google Sheets spreadsheet to enter and edit threat mitigations. Filtering updates through GitHub felt more cumbersome compared to completing our individual portions and then meeting to consolidate them into a single HTML file. Ultimately, we adapted and successfully completed the assignment.
