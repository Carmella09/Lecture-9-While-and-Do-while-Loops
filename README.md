# Lec-9-Codes


WHILE LOOP

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
      cout << "Enter a whole number: " << 
        endl; int userNum;
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
                         
   
Example                         
        
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

  

                         
