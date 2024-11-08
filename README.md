#GUESS THE NUMBER GAME

#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

int main() {

    srand(time(0));
    int r = (rand() % 10) + 1;

    cout << "Guess a number between 1 and 10\n";

    int b = 1;  
    while (true) {
        int a= 0;
        cin >> a;  

        if (a == r) {
            cout << "Hurray, you got it right!\n";
            break;  
        }
        else if (a < r) {
            cout << "Choose a number greater than " << a << "\n";
        }
        else if (a > r) {
            cout << "Choose a number lower than " << a << "\n";
        }

        b++;
    }

    cout << "You guessed the number in " << b << " attempts\n";
    
    return 0;
}
