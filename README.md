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

  
  
  
  
  
  
/*
//Nested IF example

#include <iostream>
#include <string>
using namespace std;

int main()
{

	bool zombieAtDoor = true;
	bool decideToFight = false;
	// This is the nested if-else statement that governs the decisions
	if (zombieAtDoor) {
		if (decideToFight) 
		{
			cout << "Grab a weapon and fight for your life!" << endl;
		}
		else {
			cout << "Run away, as fast as you can!" << endl;
		}
	}
	else {
		cout << "Let the civilian in" << endl;
	}
}*/
	
	
	
	
	
	
	
	//Exercise - Capital of France
#include <iostream>
using namespace std;
int main()
{
	cout << "What is the capital of France?" << endl;
	string capital;
	cin >> capital;

	if (capital == "Paris" || capital == "paris" )
	{
		cout << "You enter the correct answer";
	}
	else
	{
		cout << "Sorry you entered the wrong answere";
	}

	return 0;
}
  
	
	
	
	
	
	
	
	/*
//Exercise -Letter cheker

#include <iostream>
using namespace std;
int main()
{
	cout << "Enter an alphabet" << endl;
	string alphabet;
	cin >> alphabet;

	if (alphabet == "a" || alphabet == "e" || alphabet == "i" || alphabet == "o" || alphabet == "u")
	{
		cout << "The entered alphabet is an vowel ";
	}
	else
	{
		cout << "The entered alphabet is a constant ";
	}

	return 0;
}
*/
	
	
	
	
	
	// Exercise - Mark my Words Grade

#include <iostream>
using namespace std;

int main()
{
	cout << "Enter the marks from 1-100 to see the grade, 0 input is not accepted" << endl;
	double m;
	cin >> m;
	if (m > 70)
	{
		cout << "You have a A Grade";
	}
	else if (m >= 60 && m < 70)
	{
		cout << "You have a B Grade";
	}
	else if (m >= 50 && m < 60)
	{
		cout << "You have a C Grade";
	}
	else if (m > 40 && m < 50)
	{
		cout << "You have a D Grade";
	}
	else if (m == 40)
	{
		cout << "You have a JUST PASSED Grade";
	}
	else if (m < 40 && m != 0)
	{
		cout << "You have a Fail Grade";
	}
	else
	{
		cout << "Wrong input";
	}
}
	
	
	
	
	
	
	
	
	
	
//Exercise Starting a Band
#include<iostream>
#include<string>
using namespace std;
int main()
{
	bool musician;
	string reply;
	string instrument;
	cout << "Do you play any musical instrument? \n type 'y' for yes \n and 'n' for no \n ";
	cin >> reply;
	if (reply == "y" || reply == "Y")
	{
		musician = true;
		if (musician == true)
		{
			cout << "What kind of insturment you can play \n type d if you're a drummer \n type g if you're a guitarist\n type o for other\n" << endl;
			cin >> instrument;
			if (instrument == "g" || instrument == "G")
			{
				cout << "That's great! I really needed a guitarist." << endl;
			}
			else if (instrument == "d" || instrument == "D")
			{
				cout << "That's great! I really needed a drummer." << endl;
			}
			else if (instrument == "o" || instrument == "O")
			{
				cout << "Ah I see, actually I'm looking for guitarist or a drummer.\n Let me know if you someone who plays them\n Thank you :)" << endl;
			}
			else
			{
				cout << "Incorrect input" << endl;
			}

		}
	}
	else if (reply == "N" || reply == "n")
	{
		musician = false;
		cout << "Oh! so you don't know how to play any instrument\n it's alright, let me know if you know someone who does \n Thanks" << endl;
	}
	else
	{

		cout << "Incorrect input" << endl;
	}


	return 0;
}
	
	
	
	
	
	
	
	//Exercise - Time Killing

#include<iostream>
#include <string>
using namespace std;
int main()
{
	int time, minutes;
	cout << "Until what time your friend will come? (Enter the time in minutes)" << endl;
	cin >> time;
	if (time >= 15)
	{
		cout << "Your friend will take more or equal to 15 minutes to come,\n enter the money amount to see if you can drink something";
		cin >> minutes;
		if (minutes > 5)
		{
			cout << "You have more than 5 AED, now you will buy a drink and wait for him" << endl;
		}
		else
		{
			cout << "You don't have enough money,\n Let's just walk around";
		}
	}
	else
	{
		cout << "Your friend will be here within 15 minutes, \n so you're just going to wait for him." << endl;
	}
	return 0;
}

	
	
	
	
	
	
	
	
	
// Exercise - Earthquake
#include<iostream>
using namespace std;
int main()
{
	double mag;
	cout << "please enter the mangitude of the earthquake in numbers 0 input is not accepted : " << endl;
	cin >> mag;



	if (mag < 2.0 && mag >0) {
		cout << " earthquake is considered to be a micro earthquake.";
	}
	else if (mag >= 2.0 && mag < 3)
	{
		cout << mag << " earthquake is considered to be a very minor earthquake.";
	}
	else if (mag >= 3.0 && mag < 4)
	{
		cout << mag << " earthquake is considered to be a minor earthquake.";
	}
	else if (mag >= 4.0 && mag < 5.0)
	{
		cout << mag << " earthquake is considered to be a light earthquake.";
	}
	else if (mag >= 5.0 && mag < 6.0)
	{
		cout << mag << " earthquake is considered to be a moderate earthquake." << endl;
	}
	else if (mag >= 6.0 && mag < 7)
	{
		cout << mag << " earthquake is considered to be a strong earthquake." << endl;
	}
	else if (mag >= 7.0 && mag < 8)
	{
		cout << mag << " earthquake is considered to be a major earthquake." << endl;
	}
	else if (mag >= 8.0 && mag <= 10)
	{
		cout << mag << " earthquake is considered to be a great earthquake." << endl;
	}
	else if (mag > 10.0)
	{
		cout << mag << " earthquake is considered to be a meteoric earthquake." << endl;
	}

	else {
		cout << "You entered an invalid value" << endl;
	}
	return 0;
}
	
                                        
                                        
                                        
                                        

  
  
  
  
  
                                        
