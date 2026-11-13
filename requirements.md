**2.1 Functional Requirements**

| Requirement ID | Requirement Description | Technical Focus |
| :--- | :--- | :--- |
| FR1 | The system shall provide a web-embedded debugging and fill-in-the-blank code editor that allows users to detect wrong code and complete incomplete programming syntax and logic. | Debugging and Fill-in-the-blank Code Engine |
| FR2 | The system shall validate user-submitted code in real time and display immediate syntax error feedback or success confirmations. | Deterministic Evaluation Engine |
| FR3 | The system shall display interactive room-based scenario modules for identifying cyber threats including Phishing URLs, Malware Payloads, Online Scams and Social Engineering tactics. | Interactive Threat Rooms |
| FR4 | The system shall provide progressive, context-aware diagnostic hints when a user submits an incorrect code answer or scenario selection. | Diagnostic Hint Engine |
| FR5 | The system shall record and update user completion scores and individual skill metrics on a gamified progression dashboard upon completing a level. | Gamified Progression Dashboard|


**2.2 Non-Functional Requirements**

| Requirement ID | Quality Attribute | Description & Measurable Target |
| :--- | :--- | :--- |
| NFR1 | Performance | The deterministic evaluation engine shall validate user code submissions and display result feedback by 5 seconds. |
| NFR2 | Usability | The web application shall fully load interactive virtual room assets and layout components by 3 seconds on standard web browsers. |
| NFR3 | Reliability | The platform shall maintain its operational availability during peak educational lab hours without having heavy system crashes. |
| NFR4 | Security | The browser-embedded code engine shall safely sandbox and execute code validation without exposing backend platform files or client system vulnerabilities. |


**2.3 User stories**


<table>
  <thead>
    <tr>
      <th colspan="3" align="left">User Story 1: Real-Time Interactive Code Execution</th>
    </tr>
    <tr>
      <th align="left">Story</th>
      <th align="left">Traceability</th>
      <th align="left">Acceptance Criteria</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2" valign="top">
        As an early programmer, I want to be able to detect abnormalities in my code and complete missing syntax lines within a debugging and fill-in-the-blank web IDE and get instant error verification, so that I can learn programming logic step-by-step without suffering from mental fatigue.
      </td>
      <td valign="top">FR1</td>
      <td valign="top">
        Given a user inputs the correct syntax in the code engine, when they click submit, then the system displays a green success confirmation and unlocks the next level within 5 second.
      </td>
    </tr>
    <tr>
      <td valign="top">FR2.</td>
      <td valign="top">
        Given a user submits incorrect code syntax, when validation completes, then the system highlights the exact error line and displays a specific diagnostic error message.
      </td>
    </tr>
  </tbody>
</table>


<table>
  <thead>
    <tr>
      <th colspan="3" align="left">User Story 2: Cyber Threat Scenario Analysis</th>
    </tr>
    <tr>
      <th align="left">Story</th>
      <th align="left">Traceability</th>
      <th align="left">Acceptance Criteria</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="2" valign="top">
        As a computer science student, I want to analyse scenario-driven virtual rooms containing suspicious phishing links and social engineering conversations, so that I can develop basic practical threat pattern recognition skills.
      </td>
      <td valign="top">FR3</td>
      <td valign="top">
        Given a user enters a Phishing Threat virtual room, when inspecting a sample email script, then the system presents interactive selection options to identify malicious link parameters.
      </td>
    </tr>
    <tr>
      <td valign="top">FR4.</td>
      <td valign="top">
        Given a user fails to identify the correct threat vector twice that the user asked for help, then the system generates a progressive hint explaining the specific indicator of the part.
      </td>
    </tr>
  </tbody>
</table>



User Story 2: Cyber Threat Scenario Analysis
Story	Traceability	Acceptance Criteria
As a computer science student, I want to analyse scenario-driven virtual rooms containing suspicious phishing links and social engineering conversations, so that I can develop basic practical threat pattern recognition skills.	FR3	Given a user enters a Phishing Threat virtual room, when inspecting a sample email script, then the system presents interactive selection options to identify malicious link parameters.

	FR4	Given a user fails to identify the correct threat vector twice that the user asked for help, then the system generates a progressive hint explaining the specific indicator of the part.


User Story 3: Gamified Skill Progress Tracking
Story	Traceability	Acceptance Criteria
As a self-learner, I want to view my accumulated score points and skill progression metrics on a gamified dashboard, so that I can track my knowledge progress over time.	FR5	Given a user completes any room module or coding exercise, when navigating to the dashboard, then their updated total score and completed module badge are dynamically displayed.

		Given a user views their dashboard, when inspecting skill progression, then the system displays a breakdown of master levels across Programming Syntax, Phishing, Malware, or Social Engineering domains.



