### Updated Json Files for Faira

## Current JSON Being Used: HybridFullTable

List of all JSONs:
 - Original = The Base JSON file that was in the System to begin with
 - ComTables = First Complete Overhaul of the original.
 - EnchancedFull = A further overhaul of Constable.
 - Hybrid = A combo of Comtable and Enhanced sp that uses the better parts of each.

## Goal:
- Improve the quiering ability and interaction with Faria by improving the descriptions to make it easier for Faira to understand.

## Why:
 - Detailed Descriptions: Clear descriptions of each column help the chatbot understand the context and purpose of each data field. This makes it easier for the chatbot to provide accurate and relevant responses to user queries.
 - Defined Relationships: Including the foreign key and relational details ensures that the chatbot can accurately link related records (e.g., linking training entries to specific members).
 Status and Tracking Information: Providing information about status and update tracking helps the chatbot more effectively manage and report on the progress and changes in training records.
 - Specific Dates: Including precise details about dates (completion and expiration) allows the chatbot to give accurate timelines and reminders.

 Think of it as if you were trying to throw a ball into a basket. If it is a small basket, it is hard to throw the ball in. If it is a bigger basket, it is easier.

 ### Changes
  - August 7th, 2024, 1:52 PM: Completly redid the descriptions of everything so that they are more detailed in every way, have more clearly defined relationships with one another, and are wider so that it is easier for the chatbot to use and understand the information.

## Test Log:

---
### Question 1: A document about the Safety Procedures C-130 Hercules.

  Original JSON: Provided full details of safety procedures and general knowledge of the C-130. Along with 3 PDF Documents at the end. ----> Good

  ComTable: Provided full details of safety procedures and general knowledge of the C-130 from the PDFs. Along with 3 PDF Documents at the end. ----> Good

  EnchancedFull: Provided full details of safety procedures and general knowledge of the C-130 from the PDFs. Along with 3 PDF Documents at the end. ----> Good

  HybridFullTable:  Provided full details of safety procedures and general knowledge of the C-130 from the PDFs. Along with 3 PDF Documents at the end. ----> Good
---
### Question 2: Give me a line chart that shows the C-130's maximum payload and range limitations.

  Original JSON: Provided a chart with just the two values. We needed more prompting to get concerning one another. ----> Good

  ComTable: Provided a chart with just the two values. ----> Good

  EnchancedFullTable: Provided a chart with just the two values. ----> Good

  HybridFullTable: Provided a chart with just the two values. Included 4 PDFs. ----> Good

Notes: The issues with this prompt come from the question, not the data.
---
### Question 3: Give me a table of the combat situations the C-130 Hercules could be in.

  Original JSON: Worked well. Provided a two-column table with complete data. ----> Good

  ComTable: Worked well. Provided a two-column table with complete data. ----> Good

  EnchancedFullTable: Worked well. Provided a two-column table with complete data. ----> Good

  HybridFullTable: Worked well. Provided a two-column table with complete data. ----> Good
--- 
### Question 4: What type of training is required to maintain the C-130 Hercules?

  Orignal JSON: Work Well. Provided all data in bullet point format. ----> Good

  ComTable: Work Well. Provided all data in bullet point format. Provided 4 PDFs. ----> Good

  EnchancedFullTable: Work Well. Provided all data in bullet point format. Provided 4 PDFs. ----> Good

  HybridFullTable: Work Well. Provided all data in bullet point format. Provided 4 PDFs. ----> Good
---
### Question 5: Document of the safety Procedures for the F14 Tomcat.

  Orignal JSON: Worked Well. Provided a section on general Safety and another on Handling and Operating. Gave 5 PDFs at the end related to the topic. ----> Good.

  ComTable: Worked Well. Provided a section on general Safety and another on Handling and Operating. Gave 5 PDFs at the end related to the topic and a YouTube Video. ----> Good.

  EnchancedFullTable: Worked Well. Provided a section on general Safety and another on Handling and Operating. Gave 5 PDFs at the end related to the topic. ----> Good.

  HybridFullTable: Worked Well. Provided a section on general Safety and another on Handling and Operating. Gave 5 PDFs at the end related to the topic. ----> Good.
---
### Question 6: Give me a bar chart comparing F14 Tomcat Max Altitude to other planes we have

  Orignal JSON: Worked Well. Provided a bar chart comparing it to 4 other aircraft. (All Color Coded) ----> Good

  ComTable: Worked Well. Provided a bar chart comparing it to 10 other aircraft. (All Color Coded). Provided 33 PDFs. ----> Good

  EnchancedFullTable: Failed. Could not Provide the Information. -----> Failed

  HybridFullTable: Worked Well. Provided a bar chart comparing it to 4 other aircraft. (All Color Coded) ----> Good
---
### Question 7: Could you give me a table of the type of missions the F14 Tomcat is used for?

  Orignal JSON: Worked Well. Provided a 2-column table of the mission type and its description. ----> Good
  
  ComTable: Worked Well. Provided a 2-column table of the mission type and its description. ----> Good

  EnchancedFullTable: Worked Well. Provided a 2-column table of the mission type and its description. ----> Good

  HybridFullTable: Worked Well. Provided a 2-column table of the mission type and its description. ----> Good
---
### Question 8: How many crews are required to operate the F-14, and what are their roles?

  Orignal JSON: Worked Well. Provide a bulleted paragraph about the two roles and descriptions of what they do. ----> Good

  ComTable: Worked Well. Provide a bulleted paragraph about the two roles and descriptions of what they do. Provided 3 PDFs.  ----> Good

  August 8th JSON (EnchancedFullTable):  Worked Well. Provide a bulleted paragraph of the two roles, descriptions of what they do, and a table. Provided 3 PDFs.  ----> Good

  HybridFullTable: Provide a bulleted paragraph about the two roles and descriptions of what they do.  ----> Good
---
### Question 9: Personnel trained with the M4 question.

  Original JSON: Worked Alright. Provided a 3-column table with name, date completed, and status. However, check data to see if the completed date should be there for incomplete status. ----> Check Data

  ComTable: Worked Alright. Provided a 4-column table with name, date completed, date expired, and status. The Dates expired show that they are no longer valid and have incomplete next to them. ----> Good

  EnchancedFullTable: Worked Well. Showed two columns name and Complete status. ----> Good

  HybridFullTable: Worked Well. Provided a 4-column table with name, date completed, and date expired. ----> Good

---
### Question 10: Please give me a document about the M4 Carbine.

  Orignal JSON: Worked Well. Provided any information about the M4 in bullet point format. Included 3 PDFs at the end. ----> Good

  ComTable: Worked Well. Provided all data from the PDFs in numbered and bullet point formats. Included 3 PDFs at the end. -----> Good

  EnchancedFullTable: Worked Well. Provided all data from the PDFs in numbered and bullet point formats. -----> Good

  HybridFullTable: Worked Well. Provided any information about the M4 in bullet point format. Included 3 PDFs at the end. ----> Good
---
### Question 11: Table of combat situations for the M4 Carbine.

  Original JSON: Worked Alright. Provide a 2-column table of the situation and a description. However, the descriptions for Base Security Operations, Airfield Defense Operations, Special Defense Operations, Search and Rescue Operations, Air Base Ground Defense, and Expeditionary Operations were left Blank. ----> Bad

  ComTable: Worked Well. I fixed the formatting issue based on what was happening above. 2-column table of the situation and a description. ----> Good

  EnchancedFullTable: Worked Well. Fixed the formatting issue from what was happening above. 2-column table of the situation and a description. Provided 3 PDFs. ----> Good

  HybridFullTable: Worked Well. Fixed the formatting issue from what was happening above. 2-column table of the situation and a description. Provided 3 PDFs. ----> Good

---
### Question 12: Table of people who need to update M4 Training.

  Original JSON: Worked Alright. Provided a 3-column table with name status and completed date. However, the completed date needs to make more sense in this context. ----> Failed

  ComTable: Worked Well. Provided a one-column table for everyone who needed to update their training. Also provided the Personel Cards. ---- Good

  EnchancedFullTable: Provided a two-column table with everyone who needed it and incomplete next to their name. -----> Good

  HybridFullTable: Provided a two-column table with everyone who needed it and incomplete next to their name. -----> Good
---
### Question 13: What is the first step in handling any firearm, including the M16 rifle?

  Original JSON: Worked Well. Provided a Paragraph with all the necessary information. ----> Good

  ComTable: Worked Well. Provided a Paragraph in bullet points with all necessary information. ----> Good

  EnchancedFullTable: Worked Well. Provided a Paragraph with all the necessary information. ----> Good

  HybridFullTable: Worked Well. Provided a Paragraph with all the necessary information. ----> Good
---
### Question 14: How often should the M16 rifle be cleaned and maintained?

  Original JSON: Worked Well. Provided a Paragraph with all necessary information. ----> Good

  ComTable: Worked Well. Provided a Paragraph in bullet points with all necessary information. ----> Good

  EnchancedFullTable: Worked Well. Provided a Paragraph in bullet points with all necessary information. ----> Good

  HybridFullTable: Worked Well. Provided a Paragraph in bullet points with all necessary information. ----> Good
---
### Question 15: How do you ensure the M16 rifle is clear before loading?

  Original JSON: Worked Well. Provided a numbered guide with all necessary information. ----> Good

  ComTable: Worked Well. Provided a numbered guide with all necessary information. Provided 2 PDFs. ----> Good

  EnchancedFullTable: Worked Well. Provided a numbered guide with all necessary information. Provided 2 PDFs. ----> Good

  HybridFullTable: Worked Well. Provided a numbered guide with all nessasary information. Provided 2 PDFs. ----> Good
---
### Question 16: A table of safety procedures needed for retraining with the M249 SAW.

  Original JSON: Worked Well. Provided a 2-column table with the procedures and Descriptions. ----> Good

  ComTable: Worked Well. Provided a 2-column table with the procedures and Descriptions. Provided 2 PDFs at the end. ----> Good

  EnchancedFullTable: Worked Well. Provided a 2-column table with the procedures and Descriptions. Provided 2 PDFs at the end. ----> Good

  HybridFullTable: Worked Well. Provided a 2-column table with the procedures and Descriptions. ----> Good
---
### Question 17: Give me a bar chart of who needs to update their M249 SAW training and who doesn't.

  Original JSON: Works Well. Provided a bar chart with necessary information. Check data Though no people were "Up to Date" ----> Check Data

  ComTable: Works Well. Provided a bar chart with necessary information. There were people up to date at this time. ----> Good

  EnchancedFullTable: Worked Meh. Provided a bar chart where it listed everyone with a value of 1 or 0. ----> Meh

  HybridFullTable: Works Well. Provided a bar chart with necessary information. (Color Coded) There were people up to date this time. ----> Good
---
### Question 18: Give me a document about the Safety Procedures for the M249 SAW?

  Original JSON: Worked Well. Provided all data in a numbered and bullet point format. Included 3 PDFs related to the topic. ----> Good

  ComTable: Worked Well. Provided all data in a numbered and bullet point format. Included 3 PDFs related to the topic. ----> Good

  EnchancedFullTable: Worked Well. Provided all data in a numbered and bullet point format. Included 3 PDFs related to the topic. ----> Good

  HybridFullTable: Worked Well. Provided all data in a numbered and bullet point format. Included 1 PDF related to the topic. ----> Good
---
### Question 19: Personnel Cards for people trained with the M249.

  Original JSON: Worked Well. Provided all that was asked. ----> Good

  ComTable: Failed. Could not retrieve the data needed. -----> Failed

  EnchancedFullTable: Worked Well. Provided all that was asked. ----> Good ---> Further Testing please

  HybridFullTable: Worked Well. Provided all that was asked. ----> Good

Note: Response Recorded in FariaResponses Text File.
---
### Question 20: Give me a document about medical logistics support.

  Original JSON: Worked Well. Provided all information in bullet point format. Along with a PDF at the end. ----> Good

  ComTable: Worked Well. Provided exact lines from the PDF with the information. Provided 1 PDF at the end. -----> Good

  EnchancedFullTable: Worked Well. Provided exact lines from the PDF with the information. Provided 1 PDF at the end. -----> Good

  HybridFullTable: Worked Well. Provided exact lines from the PDF with the information. Provided 1 PDF at the end. -----> Good
---
### Question 21: What is the process for procuring medical supplies?

  Original JSON: Worked Well. Provided all information in a Numbered format. ----> Good

  ComTable: Worked Well. Provided all information in a Numbered format. Provided 1 PDF at the end. ----> Good

  EnchancedFullTable: Worked Well. Provided all information in a Numbered format. Provided 1 PDF at the end. ----> Good

  HybridFullTable: Worked Well. Provided all information in a Numbered format. Provided 1 PDF at the end. ----> Good
---
### Question 22: What procedures are in place for medical clearance before deployment?

  Original JSON: Worked Well. Provided all information in a Numbered format. Included 2 PDFs at the end. ----> Good

  ComTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good

  EnchancedFullTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good
 
  HybridFullTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good
---
### Question 23: What training is required for personnel involved in Medical Logistics?

  Original JSON: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good

  ComTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good

  EnchancedFullTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good

  HybridFullTable: Worked Well. Provided all information in a Numbered format. Included 1 PDF at the end. ----> Good
---
### Question 24: What skills do different Members have?

  Original JSON: It did not work. Provided a 2-column table (Member ID and Skill ID) and only provided the record IDs. Needs to display the the Names and the skills. ----> Failed

  ComTable: Failed. It was the same as Above for some responses but worked for other instances. ----> Failed

  EnchancedFullTable: Somewhat. Provided the Skills for five people no more. ----> Meh

  HybridFullTable: Worked. Provided all details in a 2-column table. ----> Good

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 25: Who is Grace Johnson the direct Supervisor for?

  Original JSON: Failed to find Information. -----> Failed.

  ComTable: Worked OK. Provided all Information in a line response, but it was just the name of the squadron, not any members. -----> Failed

  EnchancedFullTable:  Worked Well. Provided Squadron. I had to Prompt the members. ------> Good

  HybridFullTable: Failed. Could not Retrieve Data. ----> Failed

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 26: Who is the commander?

  Original: Failed to Find Information ----> Failed

  ComTable: Worked. Provided all Information in a line response. -----> Good

  EnchancedFullTable: Failed. Provided Wrong Information. -----> Failed

  HybridFullTable: Worked. Provided all Information in a line response. -----> Good

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 27: What are all of the groups and squadrons and who are their supervisors?

  Original: Worked Well. Provided all correct information in a 2-column table. ----> Good

  ComTable:  Worked Well. Provided all correct information in 2 2-column tables. ----> Good

  EnchancedFullTable: Worked Well. Provided all correct information in 2 2-column tables. ----> Good

  HybridFullTable: Worked Well. Provided all correct information in 2 2-column tables. ----> Good

Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 28: Who is Henry Miller's Supervisor?

  Original: Failed to Find Information ----> Failed

  ComTable:  Weird. It works sometimes, but other times failed. ----> Failed

  EnchancedFullTable: Worked Well. Provided in it in a line. -----> Good.

  HybridFullTable: Failed. I cannot get data. ----> Failed
  
Notes: Response has been Recorded in the FairaResponse Text File.
---
### Question 29: What Skills does Ethan Wilson have?

  Original: Failed to Find Information ----> Failed

  ComTable: Worked Well. Provided a 3-column table with the skill, type, and source. ----> Good

  EnchancedFullTable: Work Alright. Provided info 4/6 times. ----> Failed

  HybridFullTable: Worked Well. Provided in Bullet Point Format. ----> Good
 
Notes: Response has been Recorded in the FairaResponse Text File.

