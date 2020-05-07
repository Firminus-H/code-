# code-
second
#include <iostream>
#include <cstring>
 
using namespace std;
 
int main(int argc, const char * argv[]) {
   
    string str = "BAHASA INDONESIA";
    int i = 0;
    int size = str.size();
   
    do {
        cout << str << "\n";
       
        char c_array[size + 1];
        strcpy(c_array, str.c_str());
        str = "";
       
        if (i != 3) {
            for (int j = 0; j <= size; j++) {
                if (i == 0) {
                    if (c_array[j] != 'A') {
                        str += c_array[j];
                    }
                } else if (i == 1) {
                    if (j > 3) {
                        str += c_array[j];
                    }
                } else if (i == 2 && j < 3) {
                    str += c_array[j];
                }
            }
        }
       
