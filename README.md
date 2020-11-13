#include <cstdlib>
#include <iostream>
#include <string>

using namespace std;


int main() {
   // setlocale(LC_ALL,"Russian");
    int size=0,k=0;
    string str;
    cout<<"Введите строку:";   cin>>str;
    str+='\0';
    cout<<"Строка: "<<str<<endl;
    
    for (int i=0; str[i] != '\0'; i++) {
        size++;
    }
   
    cout<<"Длина: "<<size<<endl;
    if (size %5 == 0) {
        for (int i=0; str[i] != '\0'; i++) {
            if (str[i] == 40 || str[i] == 41 || str[i] == 91 || str[i] == 93 || str[i] == 123 || str[i] == 125) {
                k++;
            }
        }
        cout<<"\nkolvo: "<<k;
    }
    else{
        cout<<"Длина не кратна 5 "<<endl;
    }
   
    
    return 0;
}
