# challenge_globant
Section 1: API 

MySQL was used as the database engine to create the required tables, taking into consideration the structures and data types specified in the document. The SQL scripts for table creation are attached in the folder "db_project_0001". 

As part of the REST API model design, a structure was created to receive files via the API, and an insert procedure is carried out in the corresponding table based on the file name. 

Once the REST API component is available, the front-end design is integrated into the model using the streamlit tool. Given its capabilities, a logical design is created that provides an option to upload files using the Windows file explorer. Once the file is received, its name is validated, and based on the name, the REST API service is consumed to migrate data to the appropriate tables. It is clarified that in this process, a maximum data load control of 1000 records per load event was established. 

Once the data from the file is available, it is initially presented in a temporary grid for the user to visualize the data contained in each file. The user initiates the upload process by clicking the load button, and the INSERT process is confirmed. The process ends each time it reports the completion of the data load. 

Section 2: SQL 

Case 1 

A query was designed to perform counts in the specified time periods and summations for each criterion. These options are executed using the buttons in the left section of the page, in this case, "Requirement 1". The resulting data is loaded into a grid that displays the execution results. 

Case 2 

A query was designed to count the employees hired in 2021, and descending sorting is applied to the output. 

For both cases, a descriptive graph was added using the Altair graph component compatible with streamlit. These graphs visually present the behavior of each requested scenario. This graphical representation facilitates connecting with the story that these data generate over time for the company's areas. 

 
 

 
