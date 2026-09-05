# Secure Cloud Architecture Plan

Users

CDN

Load Balancer

Application Servers

Private Database


# Public and Private Resources

Resource |  Public or Private? | Explanation

CDN | Public | CND need to be public because users need to access the website through internet 

Load Balance  | Public | Load Balance need to be public because users make a requests and send it to the application server

Application Server | Private | Application Server should be private because it need to be protected from direct access from
the internet it need to be private 

Database | Private | Database it should be private because it contain a private information that only application server it should be only access by application server

# Security Controls

- IAM
The cloud environment must be accessible only by authorized users. Administrators must have more permissions to  environment while normal users can only access the function they need.
- MFA
MFA should be enable for administrators and individuals who have access to confidential information for added layer of security.
- Firewall / Security Group

- Encryption
student information should be encrypted to ensure no unauthorized people can access the confidential information.
- Logging
Every activity once login should be recorded like failed login attempts, user logins also the changes that made in the cloud should be recorded for security incidents.
- Monitoring
system needs to monitor any suspicious behavior like multiple login failures and illegal access attempts to access database.
- Backup
Database should be backup to prevent loss of student record if its happened backup record allow to restored the information if accidentally delete or corrupted.

# Principle of Least Privilege
User | Allowed Access

Administrator | Full access so it can manage the cloud and security setting

Instructor | Access to view and manage the student records

Student | Access to view their own student infromation

Developer | Developer can access the application code and development tools but limited access to database of the student

# Shared Responsibility Model

Responsibility | Cloud Provider or Customers?

Physical data center | Cloud Provider

Physical servers     | Cloud Provider

User accounts        | Customer

Student data         | Customer

IAM permissions      | Customer

Application security | Customer

Database access rules| Customer

Backups              | Customer 

1. What does Security OF the Cloud mean?
  Security Of the Cloud means the Cloud provider is responsible for ecuring the physical infrastructure lies with the cloud provider.
2. What does Security IN the Cloud mean?
   Security IN the cloud means the users are responsible on what they are put in the cloud like user account,data or any information to protect their data and resources inside the cloud
3. Which resource should be directly accessible from the Internet?
   Load balance should be direct to internet because it access the users request from the internet
4. Why should the database remain private?
  Database should remain private because it has a users private information for unauthorized users 
5. Why should users not connect directly to the database?
   Users should not connect direct to database because it can expose other student private information
6. What is the purpose of a load balancer?
   the purpose of Load balancer is to distribute other users request to other application server 
7. What happens if one application server fails?
    If the one application server fails the balancer will send a request to a working application server
8. What is the purpose of a CDN?
   The purpose of CDN is to deliver a website contents fast from a server closer location to the user. 
9. Why should administrator accounts use MFA?
    MFA is a extra protection that administrator can use to prevent unwanted people from accessing the application
10. Why should administrator access not be given to every employee?
    Administrator access is limited only the authorized person can access it because it has high level of control over the system
11. Why are logging and monitoring important?
    Logging and monitoring is important because it help to determine any security issues and suspicious behavior.
12. Why are backups important?
    Backups is important because if a document is accidentally deleted it allow student data to be restored if the document is backups

