#include <iostream>
using namespace std;

int main() {
    double temp;
    int choice;

    cout << "Choose conversion type:\n";
    cout << "1. Celsius to Fahrenheit\n";
    cout << "2. Fahrenheit to Celsius\n";
    cout << "Enter your choice (1 or 2): ";
    cin >> choice;

    cout << "Enter temperature: ";
    cin >> temp;

    if (choice == 1) {
        double result = (temp * 9 / 5) + 32;
        cout << "Temperature in Fahrenheit = " << result << endl;
    } 
    else if (choice == 2) {
        double result = (temp - 32) * 5 / 9;
        cout << "Temperature in Celsius = " << result << endl;
    } 
    else {
        cout << "Invalid choice!" << endl;
    }

    return 0;
}
