## System Administration Consultation

<br>

### Scenario 1

You’re doing systems administration work for Network Funtime Company. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Software Company**:

Network Funtime Company is a small company that builds open-source software. The company is made up software engineers, a few designers, one person in Human Resources (HR), and a small sales team. Altogether, there are 100 employees. They recently hired you as a system administrator to come in and become their IT department.

When a new person is hired on, the HR person purchases a laptop for them to do their work. The HR representative is unfamiliar with what type of hardware is out there; if a new employee requests a laptop, the HR person will purchase the cheapest option for a laptop online. Because of this, almost everyone has a different laptop model. The company doesn’t have too much revenue to spend, so they don’t order laptops until someone gets hired at the company. This leads to a few days of wait time from when someone starts to when they can actually work on a laptop.

The company doesn’t label their computers with anything, so if a computer is missing or stolen, there’s no way to audit it. There’s no inventory system to keep track of what’s currently in the fleet.

Once a computer is purchased, the HR person hands it to the new employee to set up. Software engineers that use Linux have to find a USB drive and add their preferred distribution to the laptop. Anytime someone needs something from HR -- whether it’s office related or tech related -- they email the HR representative directly.

When a new employee gets a machine, they’re given logins to use cloud services. They get a personal orientation with HR to make sure they can login. This requires the HR person to block off a few hours for every new employee. If an employee forgets the login to their machine, they have no way to retrieve a password and they have to reimagine their machine. Employees don’t have a strict password requirement to set for their computers.

The company currently has many of their services in the cloud, such as email, word processors, spreadsheet applications, etc. They also use the application, Slack, for instant communication.

**My Review**: 

> First, it's impressive that they finally hired a system administrator. hopefully, they will empower him to dispense all his fundamental duties as a system admin with best practices. While the company previously purchased low budget computers , is the earlier purchases made from a trusted Vendor? if not, that needs to be reconsidered. Although Network Funtime Company is a small company for now, they should consider setting up an enterprise account with any one of a trusted vendor; Dell and Microsoft as examples has help centers and offers long term benefits such as discounts, maintenance, repair, troubleshooting, rewards. A well structure procurement plan is also required i.e the company can adopt the right device specifications based on user needs to enable more productivity.  For example, it may be worth for spring luxury laptops for C-suite execs and dev team, midrange laptops for professional staff, and entry-level laptops for support staff.
Since the company doesn't have anything to track their inventory, moving forward, assets need to be documented and physically labelled against the value.
A directory Service is required for user and computer management. Opensource type like openLDAP can be considered since it is not OS specific. Although Microsoft active directory service is preferred on windows.  Since most of their services exists in the cloud, replication of data in the cloud are paramount.

<br><hr><br>

### Scenario 2

You’re doing systems administration work for W.D. Widgets. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Please write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Sales Company**:

W.D. Widgets is a small company that sells widgets. They’re mostly made up of salespeople who work with lots of clients. You’ve taken over as the sole IT person for this company of 80-100 people.

When HR tells you to provision a machine for a new employee, you order the hardware directly from a business vendor. You keep one or two machines in stock, in case of emergency. The users receive a username that you generate for them. You then give them an orientation on how to login when they start. You currently manage all of your machines using Windows Active Directory. The company uses only Windows computers. When a new computer is provisioned, you have to install lots of sales-specific applications manually onto every machine. This takes a few hours of your time for each machine. When someone has an IT-related request, they email you directly to help them.

Almost all software is kept in-house, meaning that you’re responsible for the email server, local machine software, and instant messenger. None of the company’s services are kept on the cloud.

Customer data is stored on a single file server. When a new salesperson starts, you also map this file server onto their local machine, so that they can access it like a directory. Whoever creates a folder on this server owns that folder and everything in it. There are no backups to this critical customer data. If a user deletes something, it may be lost for everyone.

The company generates a lot of revenue and is rapidly growing. They’re expecting to hire hundreds of new employees in the next year or so, and you may not be able to scale your operations at the pace you’re working.

**My Review**:

>
Since the company generates a lot of revenue and is rapidly growing; expecting to hire hundreds of new employees in the next year or so, it has become very important to set up  and blend a centralized management system with the existing directory service, which can be used to configure servers and manage users and computers. Configuration management tools like puppet, chef and ansible can be very helpful. 
Replication of data on and off the cloud should be adopted and a well documented disaster recovery plan should be drafted, with simulated tests carried out for several cases.


<br><hr><br>

### Scenario 3

You’re doing systems administration work for Dewgood. Evaluate their current IT infrastructure needs and limitations, then provide at least five process improvements and rationale behind those improvements. Please write a 200-400 word process review for this consultation. Remember, there’s no right or wrong answer, but make sure to provide your reasoning.

**Non-profit Company**:

Dewgood is a small, local non-profit company of 50 employees. They hired you as the sole IT person in the company. The HR person tells you when they need a new computer for an employee. Currently, computers are purchased directly in a physical store on the day that an employee is hired. This is due to budget reasons, as they can’t keep extra stock in the store.

The company has a single server with multiple services on it, a file server, and email. They don’t currently have a messaging system in place. When a new employee is hired, you have to do an orientation with them for login. You’re also responsible for installing all the software they need on their machine, and mapping the file server to their computer. The computers are managed through Windows Active Directory. When an employee leaves, they’re currently not disabled in the directory service.

The company uses an open-source ticketing system to handle all internal requests as well as external non-profit requests. But the ticketing system is confusing and difficult to use, so lots of the employees reach out to you directly to figure out how to do things. In fact, so many things are difficult to find that employees typically ask around when they have a question.

There are nightly backups in place of the file server. You store this information on a disk backup and take it home with you everyday to keep it safe in case something happens onsite. There’s also a small company website that’s hosted on the single server at the company. This website is a single html page that explains the mission of the company and provides contact information. The website has gone down many times, and no one knows what to do when it happens.

**My Review**:

> The company must ensure computers are bought from a trusted vendor even though it is a non-profit organization and there is a budget constraint. 
Each services need to be set up on their standalone server and there should be a plan for fail over. Since company don’t currently have a messaging system in place, one should be setup considering protocols like POP3, IMAP, and SMTP. It could be company specific domain server with each employees having their unique mail addresses, "firstname.lastname@company.com" as an example. A messaging technology such as Microsoft teamS can also improve communication network of their company. with the right messaging technology company will gain message security, collaboration and streamlined account controls.
When an employee leaves, company must delete their AD user account immediately, to curb leakage of sensitive data and attacks. Company needs a ticketing system that is easy to use with focus on communication and customer satisfaction, an IT ticketing system is designed to keep IT teams up to date on the status of IT tickets. technical problems can be channeled to a different pipeline and escalated to the right team so it can be resolved in a timely manner. Backups help ensure the business is kept running in the case of data loss, a hack attack or even a natural disaster. A blend of onsite and offsite backup/disaster recovery plans is optimal and ideal for the company.

<br>

**Thank you for your submission!**

An excellent response

- explains the problem or restrictions that the company faces in great detail.

- lists five or more process improvements and explains how they plan to implement each of them.

- thoroughly explains the rationale behind each improvement recommendation.

References:

* https://www.businessnewsdaily.com/9003-business-laptop-buying-guide.html
* https://smallbusiness.chron.com/keep-track-computer-inventory-18293.html
* https://www.computerweekly.com/opinion/The-problem-with-passwords-how-to-make-it-easier-for-employees-to-stay-secure
* https://www.netsfere.com/Resources/Messaging-Insights/The-Benefits-of-an-Enterprise-Messaging-System
* https://www.smartsheet.com/how-use-smartsheet-it-ticketing-system
* https://www.dobson.net/4-reasons-why-businesses-need-to-regularly-back-up-information/