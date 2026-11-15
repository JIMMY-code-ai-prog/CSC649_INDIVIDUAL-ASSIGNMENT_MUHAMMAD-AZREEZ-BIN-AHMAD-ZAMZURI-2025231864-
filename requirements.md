ID	Requirements
FR1	The system shall display a structured pre-consultation symptom questionnaire allowing patients to input active symptoms, body temperature range and symptom duration priror to Klinik Kesihatan appointment slot selection.
FR2	The system shall evaluate submitted patient symptom inputs against predefined clinical triage rules to classify the case into one of three urgency tiers either Red for emergency , Yellow for Urgent or Green for Routine
FR3	The system shall display a plain-language explanation detailing the specific red-flag symptoms that triggered the assigned risk tier alongside immediate self-care guidance.
FR4	The system shall transmit a structure pre-triage summary containing the assigned urgency tier and reported symptoms to the selected Klinik Kesihatan triage dashboard upon confirmation of a Yellow or Green booking.
FR5	The system shall diable routine Klinik Kesihatan appointment booking dor Red tier classifications and display navigation directions to the nearest hospital Emergency Department.
FR6	The system shall allow authorized Ministry of Health (KKM) clinical administrators to update symptom rules and threshold parameters through an administrative interface without modifying core application code.

Table 3.1 : Functional Requirements

ID	Quality Category	Requirements

NFR1	
Performance	The triage inference engine shall compute and render the patient’s ugency tier classification within 2 seconds of questionnaire submission under standard 4G/Wi-Fi network conditions.

NFR2	
Security & Privacy	The system shall encrypt all patient symptom records in transit using TLS 1.3 and at rest using AES-256 in compliance with Malaysia’s Personal Data Protection Act (PDPA) 2010.

NFR3	
Usability	At lest 90% of first time test users shall successfully complete the symptom triage questionnaire within 3 minutes without requiring external assistance.

NFR4	
Availability	The pre-consultation triage module shall maintain at least 99.5% operational uptime during peak public clinic operating hours which is 7:00 A.M. to 5:00 P.M.

Table 3.2 : Non-Functional Requirements
 

ID	User Story	Linked Req.	Acceptance Criteria



US1	
As a patient experiencing acute symptoms, I want to answer a quick symptoms checklist before booking a clinic slot,so that I know whether my condition requires emergency hospital care or a routine outpatient visit	


FR1,FR2,FR5	1.	Selecting “Fever > 38.5°C" and “ Persistent
vomiting” classifies the user as Red (Emergency).
2.	Standard Klinik Kesihatan appointment slot
buttons are hidden and replaced with the nearest hospital Emergency Department location and emergency hotline.



US2	
As a patient receiving a triage result, I want to see a clear explanation of why I was placed in a specific urgency tier,so that I can understand the clinical reasoning and know what immediate safety steps to take.	


FR3	1.	The result screen explicitly list the user selected
symptoms that triggered the assigned urgency tier.
2.	At least two actionable safety instructions such as oral hydration guidance and warning signs requiring immediate escalation) are displayed
below the tier badge.


US3	As a Klinik Kesihatan triage nurse, I want to view the patient’s pre-consulation symptom summary before they arrive at the clinic, so that I can prioritize ugent Yellow tier patients efficiently during registration	

FR5	1.	Confirmed bookings appear in the clinic portal Tagged with their assigned urgency badge.
2.	Selecting a patient’s booking record displays their reported summary symptoms.

Table 3 : User Stories & Acceptance Criteria
