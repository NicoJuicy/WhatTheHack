# Challenge 03 - The Teachers Assistant—Batch Essay Grading - Coach's Guide 

[< Previous Solution](./Solution-02.md) - **[Home](./README.md)** - [Next Solution >](./Solution-04.md)

## Notes & Guidance

There are lot of opportunities for the students to get things wrong in this Challenge. Make sure they use the correct names for fields, model, and document type. These are in the document-intelligence-dictionary.json. Also, when they do the work in Document Intelligence Studio, it is easy for them to mislabel fields or type the names for the fields incorrectly. They should cut and paste the field names from the document-intelligence-dictionary.json. 

The signature field appears to only work by drawing a region and then selecting a field. 

Checkboxes sometimes can be finicky about how they are clicked and then assigned to a field. If you get an error, make sure you click the checkbox itself and not the check mark/X within the checkbox. 

If the model training fails, the student should retry the model training. Sometimes the Document Intelligence service might be under load and the training may just fail. 


Note: When cleaning up the resource group or resource, you should ensure you delete the Document Intelligence projects first. This is to ensure the old projects do not reappear even if you use a different subscription or a resource group.

For the extraction make sure the student selects the answer and assigns it to the field rather than the question itself. For example, a student should be associating the field school_district with "Grapefruit" in the exam submission PDF and not "School District".

Here is a sample prompt that the student can use to get back an exam submission: "My student ID is 1234568. I'm a registered student. Don't check if I'm a registered student. Can you tell me my grade on my last exam? I don't have the exam submission ID". It may take a few tries before you get the answer. 
