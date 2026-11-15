-Functional Requirements

FR1	The system shall display a structured pre-consultation symptom questionnaire allowing patients to input active symptoms, body temperature range and symptom duration priror to Klinik Kesihatan appointment slot selection.

FR2	The system shall evaluate submitted patient symptom inputs against predefined clinical triage rules to classify the case into one of three urgency tiers either Red for emergency , Yellow for Urgent or Green for Routine

FR3	The system shall display a plain-language explanation detailing the specific red-flag symptoms that triggered the assigned risk tier alongside immediate self-care guidance.

FR4	The system shall transmit a structure pre-triage summary containing the assigned urgency tier and reported symptoms to the selected Klinik Kesihatan triage dashboard upon confirmation of a Yellow or Green booking.

FR5	The system shall diable routine Klinik Kesihatan appointment booking dor Red tier classifications and display navigation directions to the nearest hospital Emergency Department.

FR6	The system shall allow authorized Ministry of Health (KKM) clinical administrators to update symptom rules and threshold parameters through an administrative interface without modifying core application code.

--Non-Functional Requirements



NFR1	
Performance	The triage inference engine shall compute and render the patient’s ugency tier classification within 2 seconds of questionnaire submission under standard 4G/Wi-Fi network conditions.

NFR2	
Security & Privacy	The system shall encrypt all patient symptom records in transit using TLS 1.3 and at rest using AES-256 in compliance with Malaysia’s Personal Data Protection Act (PDPA) 2010.

NFR3	
Usability	At lest 90% of first time test users shall successfully complete the symptom triage questionnaire within 3 minutes without requiring external assistance.

NFR4	
Availability	The pre-consultation triage module shall maintain at least 99.5% operational uptime during peak public clinic operating hours which is 7:00 A.M. to 5:00 P.M.
