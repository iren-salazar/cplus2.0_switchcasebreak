# cplus2.0_switchcasebreak
answering were i LIVE and how many HOURS i spend in that place and the FOOD i eat

#include<iostream>
#include <stdio.h>
using namespace std;
int main()
{
  int SalazarIrenMercado;
  int house=0, apartment=0, dormitory=0;
  int place=0;
  int hour=0;
  int recommendation=0;
  
  cout<<" Where do you live? "<<"\n";
  cout<<" Choices:"<<"\n";
  cout<<" \t 1 House "<<"\n";
  cout<<" \t 2 Apartment "<<"\n";
  cout<<" \t 3 Dormitory "<<"\n";
  cout<<" Answer:"<<"\n";
  cin >> place;
  cout << "Number of hours you stay at home? \n:";
  cin >> hour;
  
  printf(" \n Residence \t No. of hours you stay at home \t Recommendation\n ");
  
  switch(place) {
    case 1: 
     cout<<" House "<<"\n";
     cout<<" \t\t  %d "<<"\n";
     
  switch(hour) {
    case 1 ... 9:
     printf("\t\t\t Snake \t"); break;
    case 10 ... 17:
     printf("\t\t\t Dog \t"); break;
    case 18 ... 20 :
     printf("\t\t\t Pot bellied pig \t"); break;
  }
  break;
  
    case 2:
     printf ( " Apartment  ");
     printf("\t\t  %d ",hour);
     
  switch(hour) {
    case 1 ... 9:
     printf("\t\t\t Hamster \t"); break;
    case 10 ... 20:
     printf("\t\t\t Cat \t"); break;
  }
  break;
    case 3: 
    printf ( " Dormitory  ");
     printf("\t\t  %d ",hour);
     
  switch(hour) {
    case 1 ... 5:
     printf("\t\t\t Ant farm \t"); break;
    case 6 ... 20:
     printf("\t\t\t Fish \t"); break;
  }
  break;
  
  default:
     printf ( " No recommendation "); break;
  }
     return 0; 
}
  /*OUTPUT:
  
  Where do you live? 
Choices:
1 House 
2 Apartment 
3 Dormitory 
Answer:
1
Number of hours you stay at home? 
:13
Residence 	 No. of hours you stay at home 	 Recommendation
  House             13                            Dog
  */
