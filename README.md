# Gov_Schemes

Overview
________________________________________

***CATEGORY – II – Gov Schemes App***

We have developed an Android App related to Government Schemes and to increase the participation of citizens in elections and government affairs.
	
*Features of the App* –

1.	All the Scheme initiated by the Government would be displayed in the app category wise like schemes 
        related to Education, Health, Rural Development, Startups etc.

2.	The users of the app can also lodge a complain which after verification will be publicly displayed in 
        the app wherein other users can also see that complain and those who are having same issue can tap the 
        plus button to increase the count of people who are suffering from the same problem.

3.	This complain will be sorted according to Location and will be available to the government officials who can then address the complain.

**ADMIN/MODERATOR PANEL**

=>      The webpage is accessible only to Admin. They can login and do the following tasks :-
        
        a. Add National/Local Scheme
        b. Validate the complains, that is Accept the legitimate and authentic complains OR delete it if found inappropriate.
________________________________________

*Technical Details* :

1.	Host Server :-  

              a.-> Hostinger   – MySQL DB
              b.-> Hostname    - ftp.hosting619.96.lt

2.	Languages and Technologies Used :

              a.Languages         –> Java, PHP( For backend and API’s), HTML,CSS,JavaScript( For Web Admin Panel )
              b.Technologies      –> Android Studio
              c.Framework/Library –> Slim for API’s, Volley for Networking , Facebook Kit for Phone No. Verification
________________________________________

* Source Code - ANDROID *  :

1.	LoginActivity.java class     -> To provide login functionalities either through phone number or email id(Facebook kit).
2.	User_verify.java class       -> For OTP verification of phone number.
3.	MainActivity.java class      -> Consisting of three tabs having fragments Scheme, Complain and Settings.
4.	SchemeFragment.java class    -> Having a Vertical View Pager Adapter to fetch scheme database from server and displaying it.
5.	ComplainFragment.java class  -> Having a list adapter to display the authentic complains.
6.	AddComplain.java class       -> To add a complain which then calls the script AddComplain.php.
7.	AppController.java class     -> For functioning of Volley HTTP Networking library.

----------------------------------------
* Source Code - WEB *  :

=>Web_Pages

1.      Login.php                    -> The Login Page for Administrator.
2.      Menu.php                     -> Has two card view like buttons for either Adding National/Local Scheme or Validating the Complains.
3.      Addscheme.php                -> Page for Adding of New Schemes.
4.      Complain.php                 -> Page for validating the complains. This fetches all the complains from the database.

=>API's/Scripts

1.      Adminlogin.php               -> Script for authenticating Login and to create a user session to prevent others from directly accesssing the webpage.
2.      Logout.php                   -> Script for the Logout button to end the user session.
3.      Accept/Decline_Complain.php  -> Script for either Accepting the complain or deleting the complain depending on Admin's Decision.
4.      News.php                     -> PHP Script using Slim Framework for various methods like to "get all schemes", "add schemes".. etc.
5.      Rpc.php                      -> Script for autocompletion of States for the page AddScheme.php.
