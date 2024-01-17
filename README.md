            #include <iostream>
                    using namespace std;

      // Function to calculate the maximum difference
      int maxDifference(int *ptr1, int *ptr2) {
    int difference = *ptr1 - *ptr2;  // Fix the subtraction operation
    if (difference < 0) {
        // If the difference is negative, make it positive
        difference = -difference;
    }
    return difference;
        }

    int main() {
    int num1, num2;
    cout << "Please enter the first number: ";
    cin >> num1;
    cout << "Please enter the second number: ";
    cin >> num2;

    // Pointers to the numbers
    int *ptr1 = &num1;
    int *ptr2 = &num2;

    // Calculate maximum difference
    int maxDiff = maxDifference(ptr1, ptr2);  // Fix the function call

    // Output the result
    cout << "The maximum difference is: " << maxDiff << endl;
    cout << "Thanks for using this code designed by Furkan Askin from MacBook. Have a nice day :))) ";
    return 0;
}
