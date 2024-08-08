### Updated Json Files for Faira

## Goal:
- Improve the quiering abilty and interaction with Faria by improving the descriptions to make it easier for Faira to understand.

## Why:
 - Detailed Descriptions: Clear descriptions of each column help the chatbot understand the context and purpose of each data field. This makes it easier for the chatbot to provide accurate and relevant responses to user queries.
 - Defined Relationships: The inclusion of the foreign key and relational details ensures that the chatbot can accurately link related records (e.g., linking training entries to specific members).
 - Status and Tracking Information: Providing information about the status and update tracking helps the chatbot to manage and report on the progress and changes in training records more effectively.
 - Specific Dates: Including precise details about dates (completion and expiration) allows the chatbot to give accurate timelines and reminders.

 Think of it as if you were trying to throw a ball into a basket. if it is a small basket then it is hard to throw the ball in. If it is a bigger basket it is easier to throw a ball in.

 ### Changes
  - August 7th, 2024, 1:52 PM: Completly redid the decriptions of everything so that they are more detailed in every way, have more clearly definded relationships with one another and are wider so that it is easier for the chatbot to use and understand the information.

## Test Log:

---
### Question 1: A document about the Safety Procedures C-130 Hercules.

Orignal JSON: Provided full details of safety procedures and general knowledge on the C-130. Along with 3 PDF Documments at the end. ----> Good

August 7th JSON:
---
### Question 2: Give me a chart that shows the What are the maximum payload and range limitations of the C-130?

Orignal JSON: Provided a chart that was just the two values. Needed more Prompting to get in relation to one another. ----> Good

August 7th JSON:

Notes: The issues with this prompt come from the question not the data.
---
### Question 3: Give me a table of the different combat situations the C-130 Hercules could be in.

Orignal JSON: Worked well. Provided a two column tables with complete data. ----> Good

August 7th JSON:
--- 
### Question 4: What type of training is required to maintain the C-130 Hercules?

Orignal JSON: Work Well. Provided all data in bullet point format. ----> Good

August 7th JSON:
---
### Question 5: Document of the safety Procedures for the F14 Tomcat.

Orignal JSON: Worked Well. Provided a section of general Safety and another on Handling and Operating. Gave 5 PDFs at the end related to the topic. ----> Good.

August 7th JSON: 
---
### Question 6: Give me a bar chart comparing F14 Tomcat Max Altitude to other planes we have

Orignal JSON: Worked Well. Provided a bar chart comapring it to 4 other aircraft. (All Color Coded) ----> Good

August 7th JSON: 
---
### Question 7: Give me a table of the type of missions the F14 Tomcat is used for.

Orignal JSON: Worked Well. Provided a 2 column table of the mission type and the Description of it. ----> Good

August 7th JSON:
---
### Question 8: How many crews are required to operate the F-14, and what are their roles?

Orignal JSON: Worked Well. Provided a bullet pointed formated paragraph of the two roles and descriptions of what they do. ----> Good

August 7th JSON:
---
### Question 9: Personnel trained with the M4 question.

Orignal JSON: Worked Alright. Provided a 3 column table with name, date completed and status. However check data to see if completed date should be there for incomple status. ----> Check Data

August 7th JSON:
---
### Question 10: Please give me a document about the M4 Carbine.

Orignal JSON: Worked Well. Provided any type of imformation about the M4 in bullet point format. Included 3 PDFs at the end. ----> Good

August 7th JSON:
---
### Question 11: Table of combat situations for the M4 Carbine.

Orignal JSON: Worked Alright. Provided a 2 column table of the situation and a description. However the description for: Base Security Operations, Airfeild Defense Operations, Special Defense Operations, Search and Rescure Operations, Air Base Ground Defense and Expeditionary Operations, were left Blank. ----> Bad

August 7th JSON:
---
### Question 12: Table of people who need to update M4 Training.

Orignal JSON: Worked Alright. Provided a 3 column table with name status and completed date. However completed date doesn't make sense in this context. ----> Bad.

August 7th JSON:
---
### Question 13: What is the first step in handling any firearm, including the M16 rifle?

Orignal JSON: Worked Well. Provided a Paragraph with all nessasary information. ----> Good

August 7th JSON:
---
### Question 14: How often should the M16 rifle be cleaned and maintained?

Orignal JSON: Worked Well. Provided a Paragraph with all nessasary information. ----> Good

August 7th JSON:
---
### Question 15: How do you ensure the M16 rifle is clear before loading?

Orignal JSON: Worked Well. Provided a numbered guide with all nessasary information. ----> Good

August 7th JSON:
---
### Question 16: A table of safety procedures needed for retraining with the M249 SAW.

Orignal JSON: Worked Well. Provided a 2 column table with the procedures and Descriptions. ----> Good

August 7th JSON:
---
### Question 17: Give me a bar chart of who needs to update their M249 SAW training and who doesn't.

Orignal JSON: Works Well. Provided a Bar chart with the nessasary Information. Check data Though no people were "Up to Date" ----> Check Data

August 7th JSON:
---
### Question 18: Give me a document about the Safety Procedures for the M249 SAW?

Orignal JSON: Worked Well. Provided all data in a numbered and bullet point format. Included 3 PDFs related to topic. ----> Good

August 7th JSON:
---
### Question 19: Personnel Cards for people trained with the M249 SAW.

Orignal JSON: Worked Well. Provided all that was asked. ----> Good

August 7th JSON:
---
### Question 20: Give me a document about medical logistics support.

Orignal JSON: Worked Well. Provided all information in bullet point format. Along with PDF at the end. ----> Good

August 7th JSON:
---
### Question 21: What is the process for procuring medical supplies?

Orignal JSON: Worked Well. Provided all information in Numbered format. ----> Good

August 7th JSON:
---
### Question 22: What procedures are in place for medical clearance before deployment?

Orignal JSON: Worked Well. Provided all information in Numbered format. Included 2 PDFs at the end. ----> Good

August 7th JSON:
---
### Question 23: What training is required for personnel involved in Medical Logistics?

Orignal JSON: Worked Well. Provided all information in Numbered format. Included 1 PDF at the end. ----> Good

August 7th JSON:
---
### Question 24: What skills do different Members have?

Orignal JSON: Did not work. Provided a 2 column table (Member ID and Skill ID) and only provided the record IDs. Needs to display the the Names and the skills. ----> Bad

August 7th JSON: Failed. Same as Above ----> Failed

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 25: Who is Grace Johnson the direct Supervisor for?

Orignal JSON: Failed to find Information. -----> Failed.

August 7th JSON: 

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 26: Who is the commander?

Orignal: Failed to Find Information ----> Failed

August 7th JSON: 

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 27: What are all of the groups and squadrons and who are their supervisors?

Orignal: Worked Well. Provided all correct information in a 2 column table. ----> Good

August 7th JSON: 

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 28: Who is Henry Miller's Supervisor?

Orignal: Failed to Find Information ----> Failed

August 7th JSON: 

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 29: What Skills does ethan Wilson have?

Orignal: Failed to Find Information ----> Failed

August 7th JSON: 

Notes: Response has been Recorded in the FairaResponse Text File.

