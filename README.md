# CIS278-Project-7-solution

Download Here: [CIS278 Project 7 solution](https://jarviscodinghub.com/assignment/cis278-project-7-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

You are writing a simple application to help Joe’s Marina keep track lending materials which are made available for marina occupants. The Marina Cafe keeps a wide selection of books and DVD’s for borrowing, and would like to automate their record keeping. The following diagrams describe the classes you will need for this project.

LendItem
– string title // title of item
– char mediumType (‘B’ or ‘D’) // book or dvd
– bool borrowed // has the item been borrowed?
– int borrowNumber // borrower’s card number
LendItem( )
LendItem(string titl, char med)
void setTitle(string manu)
void setMedium(char med)
void setBNumber(int bNumber)
void setBorrowed(bool bstatus)

bool getBorrowed()
string getTitle()
char getMedium()
int getBorrowerNumber()

virtual void printAll(ostream&)=0;
ostream& operator<<(ostream& out, const LendItem& obj) | | | | | | Book DVD - author: string - coverType: char (‘S’or ‘H’)//soft or hard - rating: string - screenType: char (‘W’or‘F’)//wide or full + Book(); + Book(string titl,string auth,char cover) + void setAuthor(string auth) + void setCover(char type) + string getAuth() + char getCover() + void printAll(ostream&) + DVD(); + DVD(string titl,string rating,char stype) + void setRating(string rate=”PG”) + void setScreen(char type) + string getRate() + char getScreen() + void printAll(ostream&) Part I (60 points) You will first need to code LendItem, Book and DVD classes. As you can see, LendItem is the base class from which the Book and DVD classes inherit. The two derived classes describe two ‘types’ of LendItems. Note that the LendItem class is an abstract class. The LendItem class provides a constructor which initializes its member variables, in addition to accessor methods for each. Each of the extending classes provide additional data members specific to the type of item, plus additional methods needed to maintain the object. The << operator overload should output the name of the item and whether it is currently borrowed or not. If it has been borrowed, the id number of the borrower is printed. Both of the derived classes provides a printAll function to printout ALL item details, included borrowed status. Part II (40 points) You are to write an APPLICATION which will allow the user to store books and DVD information. Your program should allow the user to do any of the following, until the user decides to exit: • Enter information for a new Book. This information is stored. • Enter information for a new DVD. This information is stored • borrow a Book or DVD, user provides title of item to be borrowed • print out the title and borrowed status of all Books currently stored • print out the title and borrowed status of all DVDs currently stored • accept a title as input, and output a message indicating if that item is owned by the marina, and if so, is available to borrow • accept a title as input, and output all stored information about that title • accept an author name as input, and output the title of all books by the author which are owned by the marina • output the name only of all items which are currently owned but unavailable (ie have been borrowed) Each book and DVD entered must be stored for the remainder of the program, so you will need to have an array for DVD objects and an array for Book objects. (If you want to challenge yourself, both Books and DVDs are both LendItems, so you can store all objects in one array of type LendItem* . This allows one array to be manipulated for all searches and printouts, but this solution is NOT required for this project.) You are to submit your LendItem, DVD and Book class files, in addition to the main application file.
