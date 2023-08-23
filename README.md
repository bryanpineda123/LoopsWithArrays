# LoopsWithArrays

#include <iostream>
#include <string>

using namespace std;

int main()
{

    cout << "\n\n Welcome to the demo for arrays and strings!\n\n";

    //Create a 2D Array
    int numberGrid[3][2] = //first [element][array] row/column
    {
        {1, 2},
        {3, 4},
        {5, 6}
    };

    cout << numberGrid[1][0];

    for(int i = 0; i < 3; i++)
    {
        for(int j = 0; j < 2; j++)
        {
            cout << numberGrid[i][j];
        }
        cout << endl;
    }

    // Create an int array
    int myLuckyNumbers[12];

    myLuckyNumbers[0] = 11;
    myLuckyNumbers[1] = 2;
    myLuckyNumbers[2] = 333;
    myLuckyNumbers[11] = 11111111;

    cout << "\n\n expected is 11... " << myLuckyNumbers[1] << endl;
    cout << "\n\n expected is a null value... " << myLuckyNumbers[2] << endl;
    // cout << "\n\n ?? out of bounds ?? ... " << myLuckyNumbers[12] << endl;

    // Let's code up a for loop
    for (int i = 0; i < 12; i++)
    {
        cout << "\n " << i << "  " << myLuckyNumbers[i];
    }
    cout << endl << endl;

    //Here is a 2D array:
    //3 rows, 2 columns
    int my2darray[3][2];

    //hard-code the values.
    my2darray[0][0] = 11;
    my2darray[0][1] = 12;

    my2darray[1][0] = 21;
    my2darray[1][1] = 22;

    my2darray[2][1] = 31;
    my2darray[2][2] = 32;

    // Fill my 2D array with a nested for() loop!
    int row0col0 = 71;

    for(int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 2; j++)
        {
            my2darray[i][j] = row0col0++;
        }
        //substract 2
        row0col0 = row0col0 - 2;
        row0col0 += 10;
    }

    cout << "\n\n\n";
    // Nested for loop
    for(int i = 0; i < 3; i++){
        for (int j = 0; j < 2; j++){
            cout << my2darray[i][j] << " ";
        }
        cout << "\n\n";
    }

    return 0;
}
