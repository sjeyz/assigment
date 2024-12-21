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



