# Lecture-7



//Logical AND &&

#include <iostream>
#include <string>

using namespace std;

int main()
{
	int porridgeTemperature = 56;
	if ((porridgeTemperature > 40) && (porridgeTemperature < 60))
	{
		cout << "That's just right!" << endl;
	}
	
	return 0;
}
                                        
                                        
                                        
                                        
  //Logical OR ||                                      
 #include <iostream>
#include <string>

using namespace std;

int main()
{
	bool hasVisa = false;
	bool hasDrivingLicense = true;
	if ((hasVisa == true) || (hasDrivingLicense == true))
	{
		cout << "You are permitted to drive" << endl;
	}
	else {
		cout << "Sorry, you cannot" << endl;
	}


	return 0;
}
  
  
  
  
  
  
  //Logical NOT !
#include <iostream>
#include <string>

using namespace std;

int main()
{
	int brotherA = 15;
	int brotherB = 12;
	if (!(brotherA < brotherB)) 
	{
		cout << "Brother A is older" << endl;
	}


	return 0;
}

  
  
                                        
                                        
//Using Multiple operators
#include <iostream>
#include <string>

using namespace std;

int main()
{

	bool hasVisa = false;
	bool hasDrivingLicense = true;
	bool drunk = false;
	if ((hasVisa || hasDrivingLicense) && !drunk)
	{
		cout << "You can drive" << endl;
	}
	else {
		cout << "Sorry, you can't " << endl;
	}
	return 0;
}
  
  
  
  
  
  
  //EXERCISE - THEME PARK 
#include <iostream>
#include <string>

using namespace std;

int main()
{
	double height = 0.6;
	int age = 5;

	if ((height >= 0.6) && (age >= 5))
	{
		cout << "You can ride :) " << endl;
	}
	else
	{
		cout << "You do not fulfil the requirments :(";
	}

	return 0;
}

  
  
  
  
  
  
  
  

                                        
                                        
                                        
                                        

  
  
  
  
  
                                        
