#### abstract 

###### : the summary of the project without going much deep 

What it shows:



#### what the application is,

the problem it solves,

who uses it,

its main features,

the technology or platform it runs on (briefly).



//try to focus on the problem it solves and the highlight the problem that was there before in short way 



**Functional requriements :** 



### **2. Functional requirements**



What they are: the features, meaning what the system must do. Each one describes an action or behaviour: an input, what the system does with it, and the output.



What they show: the system's functions and services. For example: "the system shall let the user log in", "the system shall transfer money", "the system shall generate a statement".



What they're used for:



Developers turn each functional requirement into a feature in the code.

Testers write at least one test case for each requirement. For example, they enter a wrong password three times and check that the account gets locked.

They become the use cases (the ovals) in your use case diagram.



Easy test: if you can ask "What does the system do?" and the requirement answers it, it's functional.



How to write them properly:



**Give each one an ID: FR-1, FR-2, FR-3…**

Use the word "shall": "The system shall…". "Shall" means compulsory.

Put one requirement per line. Don't join two features with "and".

Make it testable: specific enough that someone can check pass or fail.

Group them by module (Login, Account, Transfer…).



Example (bank app):



User registration and login



FR-1: The system shall allow a new customer to register using their account number, registered mobile number and date of birth.

FR-2: The system shall send a 6-digit OTP to the registered mobile number to verify the customer during registration and login.

FR-3: The system shall allow the customer to log in using a customer ID and password.

FR-4: The system shall lock the account after 3 consecutive wrong password attempts.

FR-5: The system shall allow the customer to reset a forgotten password after OTP verification.



Account management



FR-6: The system shall display the current balance of each of the customer's accounts.

FR-7: The system shall display the last 10 transactions on the home screen.

FR-8: The system shall allow the customer to download an account statement for a selected date range as a PDF.

#### 

#### 

#### 

#### 3\. Non-functional requirements



What they are: the qualities of the system, meaning how well it must work. They don't add a new feature. Instead, they set limits and standards on all features: speed, security, reliability, ease of use and so on.



What they show: the system's quality and constraints. Two apps can have the same features (login, transfer), but one is fast, secure and never crashes, while the other is slow and unsafe. Non-functional requirements describe that difference.



What they're used for:



Architects use them to choose the technology and design. For example, "10,000 users at once" leads to adding a load balancer and more servers.

Testers use them for performance testing, security testing and load testing.

They decide whether users actually like the app. A banking app that takes 30 seconds to load fails, even if every feature works.



Easy test: if the requirement answers "How well, how fast, how safe or how reliable?", it's non-functional.



How to write them properly:



Give each one an ID: NFR-1, NFR-2…

Group them by category. The common ones are listed in the example below.

Make them measurable with numbers. "The app should be fast" is wrong. "Each page shall load within 3 seconds" is right.

Use "shall" here too.



Example (bank app), by category:



Performance: speed and response time



NFR-1: The system shall display the account balance within 2 seconds of the request.

NFR-2: The system shall complete an IMPS or UPI transfer within 10 seconds.

