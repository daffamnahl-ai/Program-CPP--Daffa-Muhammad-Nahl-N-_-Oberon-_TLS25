# Program-CPP--Daffa-Muhammad-Nahl-N-_-Oberon-_TLS25

#include <iostream>
#include <string>

using namespace std;

void reverseString(string &s) {
    int n = s.length();
    for (int i = 0; i < n / 2; i++) {
        char temp = s[i];
        s[i] = s[n - 1 - i];
        s[n - 1 - i] = temp;
    }
}

int main() {
    string input;
    cout << "Masukkan kata : ";
    cin >> input;
    reverseString(input);
    cout <<"Hasil sandi : " << input << endl;
    return 0;
}
