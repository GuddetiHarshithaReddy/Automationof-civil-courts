# Automationof-civil-courts
                        SOFTWARE REQUIREMENT SPECIFICATIONS FOR AUTOMATION OF CIVIL COURTS
1. INTRODUCTION

1.1 Purpose 
Design a system for automating the judicial services in India. It is intended to make the whole judicial process more transparent and error free. The system removes the paper work involved in judicial process and makes bureaucratic works automated. 

1.2 Scope 
1. File the cases from plaintiffs with the help of online registration.
2. Having clear view about each and every case which was filed.
3. Able to know the status of the case i.e., pending case,proceeding case,closed cases.
4. Electronic communication with advocates.
5. Only advocates are able to file witnesses and evidences.
6. Evidence and witnesses of a particular case can be seen by plaintiffs and defendants.
7. No editing rights to public.
8. Judgement information can be seen by public.

1.3 Definition , Acronyms, and Abbreviations 
HTML: Hypertext Markup Language is a markup language used to design static web  pages. 
HTTP: Hypertext Transfer Protocol is a transaction oriented client/server protocol between web browser & a Web Server.  
HTTPS: Secure Hypertext Transfer Protocol is a HTTP over SSL (secure socket layer). 
UML: Unified Modeling Language is a general purpose, developmental, modeling language to provide a way to visualize the design of a system.
XML: eXtensible Markup Language. It is designed t store and transport data.   
PHP: Hypertext Preprocessor is a widely used, general-purpose scripting language that was originally designed for web development to produce dynamic and interactive web pages. 
 Personal details: Details of plaintiffs and defendants such as username, company, phone number, address, website, e-mail address etc.         
Contact details: Details of contact persons associated with the complain.

1.4 References 
(i) IEEE SRS Format 
(ii)  Problem Definition 

1.5 Overview       
SRS will include two sections: 
Overall Description will describe major components of the system, interconnection and  external interfaces.
Specific Requirements will describe the functions of actors, their role in the system and constraints. 
          
  

 2.GENERAL DESCRIPTION
2.1 Product Perspective  
•	The web pages (XHTML/JSP) are present to provide the user interface on customer client side. Communication between customer and server is provided through HTTP/HTTPS protocols.  
•	The Client Software is to provide the user interface on system user client side and for this TCP/IP protocols are used.  
•	On the server side web server is for EJB and database server is for storing the information.  

2.2  Product Function 
 User 1:  Court bureaucracy 
•	File Cases : 
     		Input: Details and parties involved     
			Output: Case no and date of hearing 
•	Log proceedings 
                       	Input: Case no and proceedings of the case 
                      	Output: update log  
User 2: Lawyers 
•	File evidences and witnesses 
                     	 Input : evidence and witness 
                         	 Output: update proceedings of the court 
•	View evidences and witnesses of opposite party
  		Input : Case no
   	            Output : Log of various evidences 
•	Receive formal judgement         
			Input :  Case no      
			Output : validated judgement 
User 3: Plaintiffs and Defendants
•	View case development 
      		Input : case no 
     	            Output : copy of judgement

2.3 User Characteristics  
Every user should be comfortable of working with computer and net browsing. He must have basic knowledge of English too.
  
 2.4 General Constraints 

•	GUI is only in English. 
•	Login and password is used for identification of customer and there is  no facility for guest. 
•	This system is working for single server. 
•	There is no maintainability of back up so availability will get effected. 
•	Limited to HTTP/HTTPS…
   
2.5 Assumptions and Dependencies 

•	The details related to the product, customer, payment and service transaction         provided manually. 
•	Administrator is created in the system already. 
•	Roles and tasks are predefined.  

3. SPECIFIC REQUIREMENTS
  3.1 Functional Requirements
	    3.1.1  File cases
		3.1.1.1  Introduction
				plaintiffs will file the cases against the defendants and lawyers also can file some details about the case.
		3.1.1.2  Input
				Details and parties involved.
		3.1.1.3  Processing
				when the details are given by plaintiffs or lawyers bureaucracy will register the case.
		3.1.1.4 Output
				case no and date of hearing.
	    3.1.2 Log Proceedings
		3.1.2.1  Introduction
				When the case comes under hearing some information is provided  in that hearing. For example, witnesses and evidences.
 		3.1.2.2  Input
				Case no and proceedings of the case.
		3.1.2.3  Processing
				When case no is provided then the information about the schedule is updated when it is continuing or initial hearing. If judgement is given then it is noted as closed. 			
     3.1.2.4 Output
				Update log.
  3.1.3  File evidences and witnesses
		3.1.3.1  Introduction
				Lawyers favour to plaintiffs provide evidences to the court and they  are noted.	
		3.1.3.2  Input
				Evidence and Witnesses.
		3.1.3.3  Processing
				When evidences are provided they are checked and whether  the evidences are true and updates the log.
		3.1.3.4 Output
				Log of various evidences.
   3.1.4 View evidences and witnesses of opposite party
		3.1.4.1  Introduction
				when the case no is entered then the evidences provided by the opposing party should be viewed.
		3.1.4.2  Input
				Case no.
		3.1.4.3  Processing
				when the entered  case no exists then the log appears otherwise it says invalid no.
 		3.1.4.4 Output
				Log of various evidences.
  3.1.5  Receive formal judgement
		3.1.5.1  Introduction
				When lawyers enter the case no then the judgement has to be received.
		3.1.5.2  Input
				Case no.
		3.1.5.3  Processing
				when the  case no is valid then the judgement appears otherwise it says invalid case no.
		3.1.5.4 Output
				Validated judgement.
  3.1.6  View case development
		3.1.6.1  Introduction
				When the case no is entered then the final  judgement must be displayed.
		3.1.6.2  Input
				case no.
		3.1.6.3  Processing
				when the case no entered is valid then the copy of judgement appears otherwise invalid case no.
		3.1.6.4 Output
				Copy of judgement.
						
  3.2 External interface requirments 
The user screen is divided into two horizantal panes. The first pane consists of the actions that can be done by the user. The other pane consists of case no to which the information has to be displayed.

SCREEN 1
   File Case	     Schedule	 Log Proceedings	    View Status

   CASE NO

    Submit

		
SCREEN 2
 File evidences	 View evidences	 Formal Judgement	

CASE NO.

Submit


 
SCREEN 3
 View case development

   CASE NO

    Submit

 3.3  Performance Requirements
•	The  Information page should be able to be downloaded within a minute.
•	The information must be updated  after every hearing.

3.4 Design Constraints
3.4.1 Software Languages used
The  software languages used  for coding the automation of civil courts is the AJAX for all registration forms. Other languages used are Java Server Pages (JSP), XHTML, web 2.0 is also used.
3.4.2 Developmental Tools
We will make use of developmental tools like Internet Explorer, Mozilla Firefox. Also will make use of the online references available for developing  programs in HTML.
3.4.3 Class Libraries
Will make use of the existing Java libraries available for JSP, J2EEE. Also we need to develop some new libraries for the web-based application. 

3.5 Security Requirements
Security for the purpose of this document refers to the ability of the case management system to ensure that all data elements and records remain unchanged due to unauthorized access or other human intervention, including any unauthorized addition, modification, or destruction of case management data. 
Security levels should be maintained by the user and at a minimum should allow at least 3 levels of security access to the data. Serious considerations must be given to the requirement of 4 levels of security for those courts that will allow unsecured access to viewing case information via the Internet. 
Certain security functionality is expected without identifying each function, such as the need to change passwords routinely (e.g., a predetermined number of days as determined by the system administrator and automatic “time-out” of the application after a predetermined number of minutes of inactivity). 

3.6 Maintainability Requirements
The maintenance of the system shall be done as per the maintenance contract.

3.7 Reliability Requirement:
The system has to be very reliable due to the importance of data and the damages incorrect or incomplete data can do.

3.8 Availability Requirements
The system is available 100% for the user and is used 24 hrs a day and 365 days a year. The system shall be operational 24 hours a day and 7 days a week.

3.9 Database Requirements
Database consistency is maintained over concurrent updates from multiple users by defining subsets of the database to be resource classes and locking on these logical entities . The resource classes are defined by the regions of the database .For each database transaction, including docketing, a corresponding set of resource classes is defined for locking during the update portion of that transaction.

3.10 Documentation Requirement
The documents used for the project are  .XLS, .PDF or any other desirable format is used.

3.11 Safety Requirements
The database may get crashed at any certain time due to virus or operating system failure. Therefore, it is required to take the database backup.








