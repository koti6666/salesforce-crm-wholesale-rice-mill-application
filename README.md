# salesforce-crm-wholesale-rice-mill-application
                                                     A CRM APPLICATION FOR WHOLESALE RICE MILL
                                                                        By
                                                                Kolli Koteswararao
                                                            kollikoteswararao2003@gmail.com

 
















                                                   ** Abstract**
This project, titled "A CRM Application for Wholesale Rice Mill," aims to develop a comprehensive Customer Relationship Management (CRM) system using Salesforce to streamline and enhance the operations of a wholesale rice mill. The application will integrate various Salesforce features to manage customer interactions, sales processes, and supply chain logistics efficiently. Key functionalities will include customer data management, order processing, inventory tracking, and automated communication workflows. The project will leverage Salesforce's customizable dashboards and reporting tools to provide actionable insights, enabling the rice mill to make data-driven decisions, improve customer satisfaction, and optimize overall business performance. This CRM solution will address the unique challenges of the wholesale rice industry, ensuring scalability, ease of use, and enhanced operational efficiency.

 










                                                      INDEX PAGE
Topics                                                                        page no
Object                                                                            4
Tabs                                                                             5-6
The Lightning App                                                                 7
Fields                                                                           8-11
Page layouts                                                                      12
Profiles                                                                          13
Role & Role Hierarchy                                                             14
Users                                                                            15-16
Permission sets                                                                   17
Reports                                                                          18-19
Dashboards                                                                        20

 


                                                      Objects
To manage the various entities involved in the wholesale rice mill operations, we will create four custom objects in Salesforce: Consumer, Rice Mill, Rice Details, and Supplier.
Consumer Object
The Consumer object will store detailed information about the customers purchasing rice from the wholesale mill. Fields will include Consumer Name, Contact Information, Purchase History, and Preferences. This object will help track consumer interactions, manage orders, and provide personalized service.
Rice Mill Object
The Rice Mill object will capture details about the rice mills, including Mill Name, Location, Production Capacity, and Operational Status. This object will facilitate the management of multiple rice mills, monitor their production activities, and ensure efficient operations.
Rice Details Object
The Rice Details object will maintain comprehensive information about the different types of rice available for wholesale. Fields will include Rice Type, Quality Grade, Price, Stock Levels, and Supplier Information. This object will enable easy tracking of inventory, price management, and quality control.
Supplier Object
The Supplier object will store information about the suppliers providing raw materials to the rice mills. Fields will include Supplier Name, Contact Information, Material Supplied, and Delivery Schedule. This object will help manage supplier relationships, streamline procurement processes, and ensure timely delivery of raw materials.
By creating these custom objects, the CRM application will effectively organize and manage the critical aspects of the wholesale rice mill operations, enhancing efficiency and customer satisfaction

 
                                                       Tabs
Creating Tabs for Custom Objects
In our Salesforce CRM application for wholesale rice mill operations, tabs are essential for providing users with easy access to and management of records related to key entities. We will create tabs for the Consumer, Rice Mill, Rice Details, and Supplier custom objects, enhancing usability and operational efficiency.
Consumer Tab
The Consumer tab is designed to manage customer information, including contact details, purchase history, and preferences. This tab centralizes all consumer data, making it easy for users to track interactions and manage relationships effectively. By providing a dedicated interface for consumer information, the tab supports personalized service, improves customer satisfaction, and facilitates targeted marketing efforts.
Rice Mill Tab
The Rice Mill tab offers a comprehensive view of each rice mill's details, such as location, production capacity, and operational status. This tab is crucial for overseeing the performance and activities of multiple mills, ensuring that production processes run smoothly. Users can quickly access and update information about each mill, monitor production outputs, and address any operational issues promptly, leading to better management and coordination.
Rice Details Tab
The Rice Details tab maintains detailed records of the various types of rice available for wholesale, including quality grades, pricing, stock levels, and supplier information. This tab is integral to inventory management, allowing users to monitor stock levels, manage pricing strategies, and ensure the quality of rice products. By keeping detailed rice information accessible, the tab aids in making informed decisions about procurement, sales, and inventory control.
Supplier Tab
The Supplier tab stores vital information about suppliers, such as contact details, materials supplied, and delivery schedules. This tab helps streamline procurement processes by providing a centralized repository of supplier data. Users can manage supplier relationships more effectively, ensure timely delivery of raw materials, and maintain accurate records of supplier interactions. This tab supports efficient supply chain management and helps mitigate risks associated with supply disruptions.
 
 
 
 
 
         

                                                                    The Lightning App
The "MY RICE" Lightning app is designed to optimize the management of wholesale rice mill operations by providing a streamlined and customized interface. This app integrates essential functionalities and data to enhance user productivity and efficiency.
Key Features:
Custom Branding: The app will be named "MY RICE," with personalized branding, including a custom logo and color scheme, to reflect the rice mill's identity.
Unified Navigation: It will feature tabs for important objects like Consumer, Rice Mill, Rice Details, and Supplier, allowing users quick access to relevant information and tools.
Utility Bar: The utility bar will include essential tools and utilities, such as notes and recent items, to support efficient task management.
 
 
 
 
 
                                                 Fields
When we talk about Salesforce, Fields represent the data stored in the columns of a relational database. It can also hold any valuable information that you require for a specific object. Hence, the overall searching, deletion, and editing of the records become simpler and quicker. 
Types of Fields 
Standard Fields 
Custom Fields 
Standard Fields: 
As the name suggests, the Standard Fields are the predefined fields in Salesforce that perform astandard task. The main point is that you can’t simply delete a Standard Field until it is anon-required standard field. Otherwise, users have the option to delete them at any point fromthe application freely. Moreover, we have some fields that you will find common in everySalesforce application. They are,
● Created By 
● Owner 
● Last Modified
● Field Made During object Creation
 Custom Fields: 
On the other side of the coin, Custom Fields are highly flexible, and users can change themaccording to requirements. Moreover, each organizer or company can use them if necessary. Itmeans you need not always include them in the records, unlike Standard fields. Hence, the finaldecision depends on the user, and he can add/remove Custom Fields of any given form.
Number field in rice details object
The number field allows for precise tracking of metrics crucial to inventory management and pricing strategies. For instance, the Stock Levels field helps in monitoring current inventory, while the Price per Unit field facilitates accurate pricing management.
Creating Junction Object :
A Junction  object is a custom object that serves as a bridge between two related objects in a  many-to-many relationship. It allows you to create a relationship between records of two different objects by creating a many-to-many relationship model.
Rice Details acts as a bridge, linking suppliers and rice mills with specific rice types and related information. This setup allows for detailed tracking of which suppliers provide rice to which mills and the specifics of each rice type involved.
Creating supplier name field
The Supplier Name field in the Supplier object is essential for managing supplier information effectively within Salesforce. This field serves as the primary identifier for each supplier, ensuring that each one is uniquely recognized and distinguished from others. By providing a distinct name for each supplier, it simplifies the process of locating and referencing supplier details, which is crucial for maintaining accurate and organized records.
Master-Detail Relationship between Consumer and Rice Mill Objects
This relationship allows for the management of data in a structured way, linking each rice mill directly to a specific consumer. For example, it can track which consumers are associated with which rice mills, facilitating better organization of customer preferences and mill-specific details.
Fields in supplier object
Sum of rice distributed
Adding a Sum of Rice Distributed field to the Supplier object in Salesforce allows for the aggregation of total rice distributed by each supplier. This field calculates and displays the total quantity of rice supplied across all transactions linked to the supplier.
Fields in rice details object
Rice taken
The Rice Taken field in the Rice Details object is designed to record the total amount of rice removed from inventory for various purposes.
Rice taken by shops
The Rice Taken by Shops (in Kgs) field in the Rice Details object is designed to track the quantity of rice distributed to various shops in kilograms.


                                                           Fields in consumer object
Adding the following fields to the Consumer object in Salesforce enhances the management of customer information and interactions:
First Name: Captures the consumer's first name, essential for personalized communication and record-keeping.
Last Name: Records the consumer's last name, completing the contact information and aiding in detailed identification.
Phone Number: Stores the consumer's phone number, facilitating direct contact and customer support.
Email: Keeps the consumer's email address for electronic communication and marketing purposes.
Rice Taken by Shops: Tracks the quantity of rice purchased by the consumer from various shops, providing insights into their buying patterns.
Rice Type: Identifies the specific types of rice the consumer is interested in or has purchased, aiding in inventory management and customer preferences.
Mode of Payment: Records the method used by the consumer to pay for their purchases, helping in financial tracking and reporting.

                                                            Validation rules
Improve the quality of your data using validation rules. Validation rules verify that the data a user enters in a record meets the standards you specify before the user can save the record. A validation rule can contain a formula or expression that evaluates the data in one or more fields and returns a value of “True” or “False”. Validation rules also include an error message to display to the user when the rule returns a value of “True” due to an invalid value.
Creating a validation rule for the Phone Number field in the Consumer object ensures that phone numbers entered into the system meet specific formatting and data integrity requirements.
  
                                                            
                                                            Page Layouts
Creating a Page Layout for the Consumer Object
The Consumer Layout page layout is designed to effectively organize and present key information within the Consumer object. It is structured into three distinct sections, each serving a specific purpose:
Personal Details: This section captures essential personal information about the consumer. It includes fields such as First Name, Last Name, Consumer Name, Phone Number, Email, and Rice Mill Name. Organizing these fields together provides a comprehensive view of the consumer’s identity and contact information.
Rice Details: This section focuses on information related to rice transactions. It includes fields like Rice Taken by Shop and Rice Type. This grouping helps in tracking rice consumption and preferences, facilitating better inventory and sales management.
Receipt Details: This section deals with payment information. It includes fields such as Mode of Payment and Amount Paid. By consolidating receipt-related data, it streamlines the management of financial transactions and ensures clarity in payment records.
This structured layout enhances data entry efficiency and user experience by grouping related fields, making it easier for users to access and manage critical consumer information.

                                                       
                                                       Profiles
Creating the Owner Profile
To create an Owner profile, clone the Standard User profile and name the new profile "Owner." Grant the Owner profile access permissions for the Consumers, Rice Details, Rice Mill, and Suppliers objects as specified. Save the profile settings to complete the configuration. This profile is designed to provide comprehensive access and manage critical aspects of the rice mill system.
Creating the Employer Profile
To set up an Employer profile, start by cloning the Standard Platform User profile and rename it "Employer." Configure this profile as the default for the Rice Mill application. Assign the necessary access permissions for the Consumer, Rice Details, Rice Mill, and Suppliers objects. Save the changes to finalize the profile. This profile ensures that users have the appropriate access to manage and interact with key components of the application.
Creating the Worker Profile
For the Worker profile, clone the Standard Platform User profile and designate it as "Worker." Set this profile as the default for the Rice Mill app and assign access permissions for the Consumer, Rice Details, Rice Mill, and Suppliers objects. Save the profile to complete the setup. This profile is tailored to provide specific access levels necessary for users to perform their roles effectively within the rice mill application


                        
                                                    Role & Role Hierarchy
Creating the Owner Role
The Owner role is established to grant high-level visibility and access within Salesforce. This role provides top-tier permissions, allowing users designated as Owners to manage and oversee critical records and configurations across the Salesforce system.
Creating Employer and Worker Roles
To further refine access control, two additional roles are created under the Owner role:
Employer: This role is positioned beneath the Owner and is designed for users who need to manage specific departments or functions within the organization. The Employer role provides a balanced level of access suitable for overseeing operations without the full administrative privileges of the Owner role.
Worker: Created under the Employer role, the Worker role is intended for entry-level users. It offers limited access tailored to daily tasks and operations, ensuring that users can perform their duties effectively while maintaining appropriate data security.


                                             Users
Creating Users
Activity 1: Create a User
Create a user with the following details:
First Name: Vicky
Last Name: Y
Alias: [Provide an alias]
Email ID: [Your personal email]
Username: [Username in the format: text@text.text]
Nickname: [Provide a nickname]
Role: Owner
User License: Salesforce
Profile: Owner
Activity 2: Create Additional Users
Create two more users with the following details:
User 1:
First Name: Ram
Last Name: Ram
Alias: [Provide an alias]
Email ID: [Your personal email]
Username: [Username in the format: text@text.text]
Nickname: [Provide a nickname]
Role: Employer
User License: Salesforce Platform
Profile: Standard Platform User
User 2:
First Name: Ragu
Last Name: Raj
Alias: [Provide an alias]
Email ID: [Your personal email]
Username: [Username in the format: text@text.text]
Nickname: [Provide a nickname]
Role: Worker
User License: Salesforce Platform


                                               Permission sets
A Permission Set is a collection of settings and permissions that grants users access to specific tools and functions, extending their capabilities beyond what is defined in their profiles. This flexibility allows for precise management of user permissions without altering profile settings.
Activity 1: Creating OWD Setting
Configure the Organization-Wide Defaults (OWD) to set the default internal access for the Rice Mill and Supplier objects to Public Read-Only. This setting ensures that users can view records but cannot edit them, while respecting the roles assigned within the organization.
In our configuration:
Owner roles can access records of Employer and Worker roles.
Employer roles can access records of Worker roles.
This setup maintains appropriate data visibility and control based on user roles, supporting effective permission management.
Note: To ensure comprehensive testing, create and fill out the latest 10 records in the Consumer object, making sure each field is populated. more thorough experience and evaluation of the permissions and access settings.

                                                   Reports
Reports in Salesforce provide a flexible and powerful way to analyze and visualize your data. They can be created in various styles to suit different needs, including:
Tabular Reports: These reports offer a simple list of data without subtotals. Ideal for straightforward data presentation, such as lists of accounts, contacts, or opportunities.
Summary Reports: These reports include groupings and subtotals, making them useful for hierarchical data analysis. For example, summarizing opportunities by sales stage and owner.
Matrix Reports: These allow grouping by both rows and columns, which is helpful for comparing related totals across multiple dimensions, such as summarizing opportunities by month and account.
Joined Reports: These reports combine multiple blocks of related data, each with its own columns, summaries, and filters. Useful for displaying diverse data types, such as opportunities, cases, and activities in a single view.
Activity 1: Create Report A report was created to analyze data related to Rice Mill with Consumers. It includes fields like Consumer Name, Rice Type, Rice Price/kg, Mode of Payments, and Amount Paid, and groups data by Rice Taken by Shops. This report, titled "Range of Amount per Day," helps in tracking and analyzing rice transactions.
Activity 2: Sharing Report to Owner The report was configured to send daily email notifications to the Owner. This ensures the Owner receives timely updates and can monitor the data remotely.
Activity 3: Create a Report Folder A new folder named "Estimated Rice Per Day" was created to organize reports. The "Range of Amount per Day" report was moved to this folder, facilitating easier access and management of related reports.
 
 
                                                Dashboards
Dashboards provide a visual representation of your data, helping users identify trends and make data-driven decisions.
Activity1  
 Create a new dashboard folder named "Amount Data Dashboard" to organize and manage dashboard components effectively.
Activity2:
 Build a dashboard by adding components based on selected reports. Configure the components to display data in various formats:
Vertical Bar Chart: Shows data with the X-axis as "Rice Taken by Shops" and Y-axis as the "Sum of Amount," sorted by "Rice Taken by Shops."
Donut Chart: Displays the "Range of Amount Per Day," sorted by the "Sum of Amount."
Save and finalize the dashboard to visualize and analyze the data efficiently.
.
 

