//Seneca Johnson
// Due Date: 02/23/17
// Purpose: To create a hash table to store the records using the account number key field.
// Program 4

#include <iostream>
#include <fstream>
#include <stdio.h>
#include <iomanip>
#include <sstream>
#include <cstdlib>
#include <string>
#include <ctime>

using namespace std;

int hash(const int & acct_number, const int & size)
{
   return acct_number % size;
}


struct emp_record
{
char last_name[15];
char first_name[15];
int account_num;
unsigned month; 
unsigned day;
unsigned year;
float annual_salary;
char dept_code; 
short int area_code;
short int exchange;
short int Last_4_digits; // last 4 digits of phone number
emp_record()
{
  account_num = -99;
}


}; //end struct emp_record


struct data
{
    bool collision;
    data * next;
    data()
    {
      collision = false;
    }
    if( collision == true)
      cout << "*";
  emp_record z;
};


void add( data x[], const int & key,  data & s, const int & size)
{
  emp_record = s;
  emp_record hash_table[50] = s;
  
  //builds the hash table and sets every slot equal to -99
  for( int k = 0; k < size; k++)
  { 
    hash_table[size].account_num = -99;
  }
  
  //if there is a collision
  if( hash_tabe[value] = s.account_num)
  { 
    //collision
  }
  
  hash_table[value] = s;

  //if the program goes through the above loops, then the hash table is full
  cout << "Table is full" << endl;
}  




//traverse the list to find the account number
int search( const int key, data *A[], const int size, const int account_num)
{
  data *p = A[key];
  while(p != NULL)
  {
    if( p -> key == account_num)
    {
      return account_num;
    }
    
    return account_num;
  }
}



int main()
{
  
  string month[12]={"Jan","Feb","Mar","Apr","May","June","July","Aug","Sep","Oct","Nov","Dec"};
  int total = 0;
  int size = 50;
  data a[size];
  int value;
  ifstream inF;
  ofstream outF;
  string filename;
  int falsereport, report;
  cout << "Enter filename: ";
  cin >> filename;
  outF.open("emp_record");
  inF.open(filename.c_str());
  if (inF.fail())
  {
    cout << "FATAL ERROR: Can not open file " <<  filename << endl;
    exit(1);
    
  }//if
  
  emp_record s;

  outF << setw(50) << "Employee Report" << left << endl;
  outF << setw(50) << "***************" << setw(20) << endl;
  outF << endl;
  outF << " Last" << setw(15) << "Acct" << setw(15) << "date of" << setw(15) << "annual" << setw(15) << "department" << endl;
  outF << " Name" << right << setw(20) << "Number" << setw(15) << "birth" << setw(16) << "salary" << setw(15) << "code" << setw(20) << "age" << endl;
  outF << endl;


  
  
  while( inF >> s.last_name)
  {
    
    inF >> s.first_name >> s.account_num >> s.month >> s.day >> s.year >> s.annual_salary 
             >> s.dept_code >> s.area_code >> s.exchange >> s.Last_4_digits;
    
    int value = hash(s.account_num, size);
    total += s.annual_salary;
    
    
  
    
    //Calculate the age
    time_t t = time(0);   // get time now
    struct tm * now = localtime( & t );
    /*cout << (now->tm_year + 1900) << '-' 
         << (now->tm_mon + 1) << '-'
         <<  now->tm_mday
         << endl;
    */
    int age_year = (now->tm_year + 1900) - s.year;
    //cout << age_year << endl;
    
    outF << setw(10) << s.last_name << right << setw(15) << s.account_num << setw(10) << month[s.month-1] << " " << s.day << "," << s.year << setw(10) << "$" 
         << s.annual_salary << setw(10) << s.dept_code << setw(19) << age_year << endl << endl;

  
  }
  
  outF << endl << endl << setw(50) << "TOTAL: $" << total;
 
  
  outF.open("emp_record");
  
    
}
