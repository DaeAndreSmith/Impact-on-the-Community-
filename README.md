# Impact-on-the-Community-

![image](https://user-images.githubusercontent.com/97769473/162658688-cba05862-ea83-4bdc-8829-6abcb6dcc487.png)

# The problem that exist in my community

###### The problem that exists in my community are the abandoned property in Jackson MS. The city is losing money opportunities because of the eye sore of abandoned property around the area.
 
## The sources that I used to that justified the problem
https://www.wapt.com/article/residents-fed-up-with-thousands-of-abandoned-homes-in-jackson/27374886

https://www.jacksonms.gov/blight-elimination/

https://www.wlbt.com/2020/12/22/blight-abandoned-homes-create-eyesore-jackson-residents/

http://www.city-data.com/forum/jackson/2346177-abandoned-houses-epidemic-jackson.html

https://www.jacksonfreepress.com/news/2013/jul/24/abandoned-housing-two-step/

# My soultion to the problem

###### To solve this problem I came up with the idea that the city could remodel or destory and build new property to get rid of the eye sore.
###### This will allow new people and/or businesses to move in and make money for the city.  
###### First the city will need to know where the bandon property is located.
###### Next they will need to see the condition of the property so that they can determine if the property can be remodeled or destroyed to make a new building in the same area. 
###### Finally they will need to promote the new property to help influence people and/or businesses to buy the property.
###### This will increase Jackson's profits and the city will then benefit from the increase in revenue and taxes, and these funds can then be used to improve the roads and do other much needed renovations. 

# The Code For my Solution
##
#include <iostream>
#include <string>
#include <fstream>
using namespace std;



int choice1;
int choice2;
string location;
string condition;
int bedR =0;
int bathR=0;
int BRC1 ; // new bedroom cost
int BaRC1; // bathroom remodel cost
int BRC2;
int BaRC2; 
int Sell; // price to sell property
int PI; // percent increased in profit
int i;

  class JacksonProperty
  {

  private:
string location;
string condition;


  public: 
int bedR; //bedrooms
int bathR; // bathrooms
     };

class House: public JacksonProperty {
public:
  float getNewPCost() //New property cost
{
return 15000 + 30000 +  BRC1  + BaRC1; // 15000 average deconstruction cost
  // 30000 cost to build the new property and other item in it
    }

float getRePCost() // Remodel property cost
{ 
  return BaRC2 + 11000 + BRC2; // 11000 the average cost to remodel other place in the property
}
};

int main() {
    House NewHouse;
  for (int i = 0; i < 2; i++){
    cout<< i<< '\n' << endl;
  
         
cout << "Hello welcome to Abandoned Property Remodeler" << '\n' << "If you watn to stop this program enter 1." <<'\n' <<"If you want to continue enter 2. " << endl;
  cin >> choice1;

if (choice1 == 1) {
        
      cout << "You have chosen 1 Thank you for your time. " << endl;

  return 0;
  
  } 
else if (choice1 == 2) { 
  
  cout << "Please enter the location of the abanonded property." << endl; 
cin >> location;
  
cout<<'\n'<< endl;
  
  cout << "Please enter the condition of the property." << endl;
  cin >> condition;
  
  cout<<'\n'<< endl;
  }
  cout << "If you want to remodel the property please enter 1." << '\n'<< "If you want to construnct a new building in that area please enter 2."<< '\n' << "Please enter 3 to end program. "<< endl;
cin >> choice2;
  
  if (choice2 == 1) {
        
    cout << "How many bedroom will this property have. " << endl;
    cin >> bedR;

    cout << "How many bathroom will this property have. " << endl;
    cin >> bathR;
 
BRC1 = (10300*bedR);
BaRC1 = (7600 * bathR); 

   
    cout << "This will cost you $"<< NewHouse.getNewPCost() << " to destory and build this property. " << endl;
    
    cout<< "How much will you sell this property for?"<<endl;
    cin >> Sell;
    
    PI=((Sell -NewHouse.getNewPCost())/NewHouse.getNewPCost())*(100);
   
    cout << "You have made " << PI<<"% from this property."<<endl;
    
  } else if (choice2 == 2) { 
      cout << "How many bedroom do this property have. " << endl;
    cin >> bedR;

    cout << "How many bathroom do this property have. " << endl;
    cin >> bathR;
    
   BRC2 =(6500*bedR);
    BaRC2 =(5000*bathR);
    
cout << "This will cost you $"<< NewHouse.getRePCost() << " to remodel this property. " << endl;

cout<< "How much will you sell this property for?"<<endl;
    cin >> Sell;
    
    PI=((Sell -NewHouse.getRePCost())/NewHouse.getRePCost())*(100);
    cout << "You have made " << PI<<"% from this property."<<endl;
   }
    
  else {  
    
  cout << "You have chosent to end this program Thank You" << endl;

    }
  return 0;  
    }
  return 0;  
  };
