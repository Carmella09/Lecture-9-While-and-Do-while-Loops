# Lec-9-Codes

//EXERCISE BREAK

Exercise: While Loop

Reverse 9 times table

        #include <iostream>  
        using namespace std;

        int main()
        {
            int num = 108;

            while (num >= 9)  
            {
                cout << num << endl;
                num = num - 9;
            }

            cin.get(); 
            return 0;
        }


The Pointless Box

        #include <iostream>
        using namespace std;
        int main()
        {

            cout << "Enter either 1 or 2 only: \n";
            int number;
            cin >> number;
            while (number != 0 && number <= 2 && !cin.fail())
            {
                if (number == 1)
                {
                    cout << "You have enter number 1. \n";
                }
                else
                {
                    cout << " you have enter number 2. \n";
                }

                cout << " Enter either 1 or 2 \n";
                cin >> number;

            }

            cout << "You did not enter the number 1 or 2.";

        }

    

Exercise: Do While Loop
                         
Input improvement

        #include <iostream>
        using namespace std;
        int main() {
            char input;
            do {
                cout << "Would you like to Quit (Y/N)?" << endl;
                cin >> input;
            } while 
                ((input != 'Y') && (input != 'y'));
            return 0;
        }


Brute-Force Attack

        #include <iostream>
        using namespace std;
        int main()
        {
            string password = "246";
            string userInput;

            while (userInput != password)
            {
                cout << "Enter the pass code for the safe" << endl;
                cin >> userInput;

            }

            cout << "hello there";
        }


Brute-Force Attack II

        #include <iostream>
        using namespace std;
        int main()
        {
            string password = "246";
            string pass;
            int x = 5;


            while (x > 0)
            {
                cout << "\nYou can only have 5 tries and if you fail you'll get bonk." << endl;
                cout << "Passcode: " ;
                cin >> pass;
                if (pass == password)
                {
                    cout << "\nWelcome 'Username' " << endl;

                    break;
                }
                else
                    x--;
            }
            if (x == 0)
            {
                cout << "\nGet ready to be bonk!" << endl;
            }
        }
    

Input Improvement 

        #include <iostream>
        using namespace std;
        int main() {
            char input;
            do {
                cout << "Would you like to Quit (Y/N)?" << endl;
                cin >> input;
            } while 
                ((input != 'Y') && (input != 'y'));
            return 0;
        }


Loopy

        #include <iostream>  
        using namespace std;
        int main() {

            int myInt = 0;
            int counter;

            cout << "Enter a number: " << endl;
            cin >> counter;
            do
            {
                cout << myInt << endl;
                myInt++;

            } while (myInt <= counter);

        }

//NOT EXERCISE

LOOP

WHILE LOOPS

while loops Example

    #include <iostream>
    using namespace std;
    int main()
    {
      int count = 1;
      while (count <= 1000) {
        cout << count << endl;
        count++;
      }
    }
                         
                         
Break Example
                         
    #include <iostream>
    using namespace std;
    int main()
    {
      cout << "Enter a whole number: " << endl; 
      int userNum;
      cin >> userNum;

      int count = 1;
      while(true){
        cout << count << endl;
        if (count == userNum) {
          break;
        }
        count++;
      }

    }
  
  
Alternative to previous Break Solution
  
    #include <iostream>
    using namespace std;
    int main()
    {
      cout << "Enter a whole number: " << endl; 
      int userNum;
      cin >> userNum;

      int count = 1;
      while(count <= userNum){
        cout << count << endl;
        count++;
      }

    }
                         
   
While Loop error check Example                         
        
    #include <iostream>
    using namespace std;
    int main()
    {
      cout << "Enter your age: " << endl; 
      int age;
      cin >> age;

      while(cin.fail())
      {
        cout << "Invalid input.\nPlease enter a valid age" << endl;
        cin.clear();
        cin.ignore(1000,'\n');
        cin >> age;
      }
      cout << "Your age is: " << age;
    }
 
  
Remain Positive
                         
    #include <iostream>
    using namespace std;
    int main()
    {
      float myNum = 20;
      while (myNum > 0) {
        cout << myNum << endl;
        myNum = myNum - 0.5;
      }

    }
  
  
DO WHILE LOOPS
  
Login Do While Example
  
    #include <iostream>
    using namespace std;
    int main()
    {
      string password = "1234password";
      string userInput;

      do {
        cout << "Enter your Password" << endl;
        cin >> userInput;
      } while (password != userInput);

      cout << "Welcome to the super secure banking area" << endl;
    }
  
  
Login While Alternative
  
    #include <iostream>
    using namespace std;
    int main()
    {
      string password = "1234password";
      string userInput;

      cout << "Enter your Password" << endl;
      cin >> userInput;

      while (password != userInput) 
      {
        cout << "Enter your Password" << endl;
        cin >> userInput;
      }

      cout << "Welcome to the super secure banking area" << endl;
    }

  


