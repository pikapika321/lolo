#include<iostream>

#include<cstring>

#include<cstdlib>

#include<iomanip>

#include<cstdio>

#define max 20

using namespace std;

struct employee

{

 char name[20];

 long int code;

 char designation[20];

 int exp;

 int age;

};

int num;

employee emp[max],tempemp[max],sortemp[max],sortemp1[max];

int main()

{


 void build();

 void list();

 void insert();

 void deletes();

 void edit();

 void search();

 char option;

 void menu();

menu();

while((option=cin.get())!='q')

 {

  switch(option)

  {

   case '1':

         build();

         break;

   case '2':

         list();

         break;

   case '3':

         insert();

         break;

   case '4':

         deletes();

         break;

   case '5':

       edit();

        break;

   case '6':

        search();

        break;


  }


   menu();
}

  return 0;

 }

 void menu()

 {

cout<<"          ";

printf("\n*****  Employees Management System ***** ");





cout<<endl;

cout<<"             ";

cout<<"\n\t\t Press  1---->Built The Employee Table ";

cout<<"             ";

cout<<"\n\t\t Press  2---->List The Employee Table  ";

cout<<"             ";

cout<<"\n\t\t Press  3---->Insert New Entry        ";

cout<<"             ";

cout<<"\n\t\t Press  4---->Delete An Entry         ";

cout<<"             ";

cout<<"\n\t\t Press  5---->Edit An Entry           ";

cout<<"             ";

cout<<"\n\t\t Press  6---->Search Arecord          ";

cout<<"             ";

cout<<"\n\t\t Press  q---------->Quit Program              ";

cout<<"             ";

cout<<"\n\n \t\t Select Your Option Please ====> ";

}


void build()

{






 printf("Build The Table");

 cout<<endl;

 ;

 cout<<"maximum number of entries  -----  >  20"<<endl;

 cout<<"how many do you want    ----->";

 cin>>num;

 cout<<"Enter The Following Items"<<endl;

 for(int i=0;i<=num-1;i++)

 {

  cout<<" Name  ";

  cin>>emp[i].name;

  cout<<"Code  ";

  cin>>emp[i].code;

  cout<<"Designation  ";

  cin>>emp[i].designation;

  cout<<"Years of Experience  ";

  cin>>emp[i].exp;

  cout<<"Age  ";

  cin>>emp[i].age;

 }

  cout<<"going to main menu";



}


void  list()

{





 printf("       ********List The Table********");

 cout<<endl;

 

 cout<<"     Name     Code     Designation     Years(EXP)     Age "<<endl;

 cout<<"    ------------------------------------------------------"<<endl;

 for(int i=0;i<=num-1;i++)

 {

  cout<<setw(13)<<emp[i].name;

  cout<<setw(6)<<emp[i].code;

  cout<<setw(15)<<emp[i].designation;

  cout<<setw(10)<<emp[i].exp;

  cout<<setw(15)<<emp[i].age;

  cout<<endl;

 }

  cout<<"going to main menu";

 

  }

  void insert()

  {


  int i=num;

  num+=1;

 

  printf("Insert New Record");

  cout<<endl;

  

  cout<<"Enter The Following Items"<<endl;

  cout<<"Name  ";

  cin>>emp[i].name;

  cout<<"Code  ";

  cin>>emp[i].code;

  cout<<"Designation  ";

  cin>>emp[i].designation;

  cout<<"Years of Experience  ";

  cin>>emp[i].exp;

  cout<<"Age  ";

  cin>>emp[i].age;

  cout<<endl<<endl;

  cout<<"going to main menu";

 


  }



  void deletes()

  {


  

   int code;

   int check;

   printf("Delete An Entry");

   

   cout<<endl;

   cout<<"Enter An employee Code To Delete That Entry  ";

   cin>>code;

   int i;

   for(i=0;i<=num-1;i++)

   {

    if(emp[i].code==code)

    {

      check=i;

    }

   }

   for(i=0;i<=num-1;i++)

   {

    if(i==check)

    {

    continue;

    }

    else

    {

    if(i>check)

    {

     tempemp[i-1]=emp[i];

    }

    else

    {

     tempemp[i]=emp[i];

    }

     }

   }

  num--;


  for(i=0;i<=num-1;i++)

  {

   emp[i]=tempemp[i];

  }

 }


void edit()

{


 int jobcode;



 printf("          Edit An Entry           ");

 cout<<endl;

 cout<<endl;

 int i;

 void editmenu();

 void editname(int);

 void editcode(int);

 void editdes(int);

 void editexp(int);

 void editage(int);

 char option;

 

 cout<<"Enter An employee code To Edit An Entry----  ";

 cin>>jobcode;

  editmenu();

 for(i=0;i<=num-1;i++)

   {

    if(emp[i].code==jobcode)

    {


while((option=cin.get())!='q')

{

      switch(option)

      {

       case 'n':

            editname(i);

            break;

       case 'c':

            editcode(i);

            break;

       case 'd':

            editdes(i);

            break;

       case 'e':

            editexp(i);

            break;

       case 'a':

           editage(i);

           break;

     }

   editmenu();

    }

  }

  }

  }

  void editmenu()

  {


   cout<<"        What Do You Want To edit";

   cout<<"          n--------->Name ";

   cout<<"          c--------->Code ";

   cout<<"          d--------->Designation";

   cout<<"          e--------->Experience ";

   cout<<"          a--------->Age        ";

   cout<<"              q----->QUIT                            ";

   cout<<"   Options Please ---->>>  ";

  }

  void editname(int i)

  {

     cout<<"Enter New Name----->  ";

     cin>>emp[i].name;

  }

  void editcode(int i)

  {

   cout<<"Enter New Job Code----->  ";

   cin>>emp[i].code;

  }

  void editdes(int i)

  {

   cout<<"enter new designation----->  ";

   cin>>emp[i].designation;

  }

  void editexp(int i)

  {

   cout<<"Enter new Years of Experience";

   cin>>emp[i].exp;

  }

  void editage(int i)

  {

   cout<<"Enter new Age ";

   cin>>emp[i].age;

  }


void search()

{



 

  printf("Search an employee...");

  

  cout<<endl;

  cout<<endl;

  int jobcode;


  cout<<"Enter Code Of An Employee                    ";

 cin>>jobcode;

 for(int i=0;i<=num-1;i++)

   {

    if(emp[i].code==jobcode)

    {


    cout<<"       Name     Code     Designation     Years(EXP)     Age "<<endl;

 cout<<"       ------------------------------------------------------"<<endl;

  cout<<setw(13)<<emp[i].name;

  cout<<setw(6)<<emp[i].code;

  cout<<setw(15)<<emp[i].designation;

  cout<<setw(10)<<emp[i].exp;

  cout<<setw(15)<<emp[i].age;

  cout<<endl;

 }


  }

    cout<<"going to main menu";

 



}
