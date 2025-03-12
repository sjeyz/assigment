#include <iostream>
using namespace std;

// Function declarations
void sum();
void subruction();
void multipley();
void divide();

int main() {
    int n;
    cout << "Press 1 for addition" << endl;
    cout << "Press 2 for subtraction" << endl;
    cout << "Press 3 for division" << endl;
    cout << "Press 4 for multiplication" << endl;
    cin >> n; // Take input for the choice
    
    if (n == 1) {
        sum();
    } else if (n == 2) {
        subruction();
    } else if (n == 3) {
        divide();
    } else if (n == 4) {
        multipley();
    } else {
        cout << "Invalid option." << endl;
    }
    return 0;
}
#include <iostream>
#include <cmath>

bool checkPowerEquality(double base, double exponent, double target) {
    return std::abs(std::pow(base, exponent) - target) < 1e-9;
}

int main() {
    double num1, num2, num3;
    std::cin >> num1 >> num2 >> num3;
    if (checkPowerEquality(num1, num2, num3)) {
        std::cout << "True\n";
    } else {
        std::cout << "False\n";
    }
    return 0;
}

#include<iostream>
using namespace std;
int main(){ //main function
  cout<<"DO you want the play the game ? (y,n)";
  string response;
  cin>>response;
  cout<<"you enter"<<""<<response<<endl;
  if(response == "y"){
  	cout<<"let play the game, then.../n";
  }

// Function definitions
void sum() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The sum is: " << num1 + num2 << endl;
}

void subruction() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The subtraction is: " << num1 - num2 << endl;
}

void multipley() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The multiplication is: " << num1 * num2 << endl;
}

void divide() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    if (num2 != 0) {
        cout << "The division result is: " << num1 / num2 << endl;
    } else {
        cout << "Error: Division by zero is not allowed." << endl;
    }
}
#include <iostream>
#include <cmath> 

bool isPerfectSquare(int number) {
    if (number < 0) {
        return false; 
    }
    int root = static_cast<int>(sqrt(number)); 
    return root * root == number;
}

int main() {
    int number;

    std::cout << "Enter a number: ";
    std::cin >> number;

    if (isPerfectSquare(number)) {
        std::cout << number << " is a perfect square." << std::endl;
    } else {
        std::cout << number << " is not a perfect square." << std::endl;
    }

    return 0;
}

#include <iostream>
using namespace std;

int main() {
    int num, originalNum, reversedNum = 0, remainder;
    cout << "Enter a number: ";
    cin >> num;
    originalNum = num;
    while (num > 0) {
        remainder = num % 10;
        reversedNum = reversedNum * 10 + remainder;
        num /= 10;
    }
    if (originalNum == reversedNum) {
        cout << originalNum << " is a palindrome." << endl;
    } else {
        cout << originalNum << " is not a palindrome." << endl;
    }
    return 0;
}
#include <iostream>
#include <cmath> // For the pow function
using namespace std;

// Function to calculate the power of a number
double power(double base, int exponent = 2) {
    return pow(base, exponent);
}

int main() {
    double n;
    int p = 2; // Default value for the exponent

    // Prompt for the base
    cout << "Enter the base (n): ";
    cin >> n;

    // Prompt for the exponent (optional)
    cout << "Enter the exponent (p) (or press Enter for default 2): ";
    if (cin.peek() != '\n') { // Check if the user enters something
        cin >> p;
    }

    // Call the power function and display the result
    double result = power(n, p);
    cout << "The result of " << n << " raised to the power " << p << " is: " << result << endl;

    return 0;
}
#include <iostream>
#include <cmath>

bool checkPowerEquality(double base, double exponent, double target) {
    return std::abs(std::pow(base, exponent) - target) < 1e-9;
}

int main() {
    double num1, num2, num3;
    std::cin >> num1 >> num2 >> num3;
    if (checkPowerEquality(num1, num2, num3)) {
        std::cout << "True\n";
    } else {
        std::cout << "False\n";
    }
    return 0;
}
#include <iostream>

int main() {
    int rows = 5; 
    for (int i = rows; i > 0; --i) {
        for (int j = 0; j < i; ++j) {
            std::cout << "*";
        }
        
#include <iostream>

int main() {
    int rows = 5; 
    for (int i = rows; i > 0; --i) {
        for (int j = 0; j < i; ++j) {
            std::cout << "*";
        }
        
        std::cout << std::endl;
    }

    return 0;
}
#include <iostream>
#include <cmath> 

bool isPerfectSquare(int number) {
    if (number < 0) {
        return false; 
    }
    int root = static_cast<int>(sqrt(number)); 
    return root * root == number;
}

int main() {
    int number;

    std::cout << "Enter a number: ";
    std::cin >> number;

    if (isPerfectSquare(number)) {
        std::cout << number << " is a perfect square." << std::endl;
    } else {
        std::cout << number << " is not a perfect square." << std::endl;
    }

    return 0;
}
#include <iostream>
using namespace std;

int main() {
    int num, originalNum, reversedNum = 0, remainder;
    cout << "Enter a number: ";
    cin >> num;
    originalNum = num;
    while (num > 0) {
        remainder = num % 10;
        reversedNum = reversedNum * 10 + remainder;
        num /= 10;
    }
    if (originalNum == reversedNum) {
        cout << originalNum << " is a palindrome." << endl;
    } else {
        cout << originalNum << " is not a palindrome." << endl;
    }
    return 0;
}


#include <iostream>
#include <cmath> // For the pow function
using namespace std;

// Function to calculate the power of a number
double power(double base, int exponent = 2) {
    return pow(base, exponent);
}

int main() {
    double n;
    int p = 2; // Default value for the exponent

    // Prompt for the base
    cout << "Enter the base (n): ";
    cin >> n;

    // Prompt for the exponent (optional)
    cout << "Enter the exponent (p) (or press Enter for default 2): ";
    if (cin.peek() != '\n') { // Check if the user enters something
        cin >> p;
    }

    // Call the power function and display the result
    double result = power(n, p);
    cout << "The result of " << n << " raised to the power " << p << " is: " << result << endl;

    return 0;
}
#include <iostream>
#include <cmath>

bool checkPowerEquality(double base, double exponent, double target) {
    return std::abs(std::pow(base, exponent) - target) < 1e-9;
}

int main() {
    double num1, num2, num3;
    std::cin >> num1 >> num2 >> num3;
    if (checkPowerEquality(num1, num2, num3)) {
        std::cout << "True\n";
    } else {
        std::cout << "False\n";
    }
    return 0;
}
Question:6
#include <iostream>

bool isPalindrome(int number) {
    int originalNumber = number;
    int reversedNumber = 0;

    while (number > 0) {
        int digit = number % 10;
        reversedNumber = reversedNumber * 10 + digit;
        number /= 10;
    }

    return originalNumber == reversedNumber;
}

int main() {
    int num;

    std::cout << "Enter a number: ";
    std::cin >> num;

    if (isPalindrome(num)) {
        std::cout << num << " is a palindrome." << std::endl;
    } else {
        std::cout << num << " is not a palindrome." << std::endl;
    }

    return 0;
}

   #include <iostream>
#include <cmath> 
using namespace std;

double calculateArea(double radius) {
    return M_PI * radius * radius;
}

int main() {
    double radius;

    cout << "Enter the radius of the circle: ";
    cin >> radius;

    double area = calculateArea(radius);

    cout << "The area of the circle is: " << area <<endl;

    return 0;
}


#include <iostream>
#include <string>

void displayName(const std::string &name) {
    std::cout << "Hello, " << name << "!" << std::endl;
}

int main() {
    std::string userName;

    std::cout << "Enter your name: ";
    std::getline(std::cin, userName);

    displayName(userName);

    return 0;
}
#include <iostream>

void swap(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}

int main() {
    int num1, num2;

    std::cout << "Enter two integers: ";
    std::cin >> num1 >> num2;

    std::cout << "Before swapping: num1 = " << num1 << ", num2 = " << num2 << std::endl;

    swap(num1, num2);

    std::cout << "After swapping: num1 = " << num1 << ", num2 = " << num2 << std::endl;

    return 0;
}
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Style</title>
  <link rel="stylesheet" href="project.css">
</head>
<body>
  <h1>This is heading one</h1>
  <p>
    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Odit a molestias porro voluptates at, hic placeat dignissimos officia .
  </p>
  <h1>something in the heading</h1>
  <h1> something in the heading</h1>
  <button>cilck me </button>
</body>
</html>#include<iostream>
using namespace std;
class student{
	public:
	string name;
	string deperment;
	int rollno;
	double cgp;
};
int main(){
	student s1;
	s1.name = "sawera";
	s1.rollno = 034;
	s1.cgp = 8.9;
	s1.deperment = "Bsse 1b";
	cout<<s1.name<< " "<<s1.cgp<<" "<<s1.deperment<<" "<<s1.rollno<<endl;
	
	student s2;
	s1.name = "Aliza";
	s1.rollno = 005;
	s1.cgp = 6.9;
	s1.deperment = "Bsse 1b";
	cout<<s1.name<< " "<<s1.deperment<<" "<<s1.rollno<<" "<<s1.cgp<<endl;
	
	return 0;
}

#include<iostream>
using namespace std;
class car{
	public:
	string name;
	double price;
	string type;
	string seats;
	;
};
int main(){
	car c1;
	c1.name ="honda City";
	c1.price = 85000;
	c1.type = "sendan";
	c1.seats = "two seater";
	cout<<c1.name<<endl;
	cout<<c1.type<<endl; 
	cout<<c1.price<<endl; 
		cout<<c1.seats<<endl;
		cout<<"***************************************"<<endl;
		car c2;
	c2.name ="parder";
	c2.price = 102000;
	c2.type = "sendan";
	c2.seats = "two seater";
	car c3;
	c3.name ="BNW";
	c3.price = 24007000;
	c3.type = "sendan";
	c3.seats = "four seater";
	cout<<c2.name<<endl;
	cout<<c2.type<<endl; 
	cout<<c2.price<<endl; 
		cout<<c2.seats<<endl; 
		cout<<"************************************************"<<endl; 
			cout<<c3.name<<endl;
	cout<<c3.type<<endl; 
	cout<<c3.price<<endl; 
		cout<<c3.seats<<endl; 
		cout<<"**************************************************"<<endl; 
		return 0;
}
#include<iostream>
using namespace std;
 class student{
 	public:
 	string name;
 	string depertment;
 	int rollno;
 	double cgp;
 	
 student(string s, string b,int r,double c){
	name = s;
	rollno = r;
	cgp = c;
	depertment = b;
}
};
int main(){
	student s1("sawera", "bsse",34,3.4);
	cout<<"student name :"<<s1.name<<endl;
	cout<<"student depertment:"<<s1.depertment<<endl;
	cout<<"student rollno:"<<s1.rollno<<endl;
	cout<<"student cgp:"<<s1.cgp<<endl;
	return 0;
}
