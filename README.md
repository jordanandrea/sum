# sum
This project takes the sum of all the numbers it takes to get to the entered integer. For example, if the user input 3, it will take the sum of 1+2+3.

#include <stdio.h>
#include <iostream>
using namespace std;

int main()
{
    //declare variables
    int num, sum;
    
    //ask user for a number
    cout << "Enter a positive integer." << endl;
    cin >> num;
    
    //DO NOT take a negative integer
    while (num < 0){
    cout << "ERROR: NUMBER MUST BE POSITIVE" << endl;
    cout << "Enter a positive integer" << endl;
    cin >> num;
    }
    
    //use loop to get sum of all integers from 1 to one entered
    for (int i = 1; i <= num; i++){
       sum +=i; 
    }
    
    cout << "The sum is " << sum << endl;
    
    return 0;
}

