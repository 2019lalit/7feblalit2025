//1.Write a program to count the number of digits in a given number n.
//n = 12345
//5
#include<bits/stdc++.h>
using namespace std;
int Number(int num){
    int count=0;
    while(num>0){
      
        num=num/10;
        count++;
    }
    return count;
}
int main(){
    int num;
    cout<<"please enter the number"<<endl;
    cin>>num;
    Number(num);
    cout<<Number(num);
    return 0;
}

--------------------------------------------------------------------------------------------------------
//2.Write a program to count how many times a digit d appears in the number n.

//n = 121212, d = 2
//3
#include<bits/stdc++.h>
using namespace std;

int countD(int n, int d) {
    int count = 0;
    while (n > 0) {
        if (n % 10 == d) { 
            count++;
        }
        n /= 10; 
    }
    return count;
}

int main() {
    int n;
    cout<<"please enter a number"<<endl;
    cin>>n;
    int d;
    cout<<"please enter number which we count"<<endl;
    cin>>d;
    
    

    cout << "The digit " << d << " appears " << countD(n, d) << " times in " << n << endl;
    return 0;
}

-------------------------------------------------------------------------------------------------------

//Sum of all digits
// number 12345     sum of all digit:- 15
#include <iostream>
using namespace std;

int lalit(int n) {
    int sum = 0;
    while (n > 0) {
        sum = sum + (n % 10); 
        n = n/10;      
    }
    return sum;
}

int main() {
    int n;
    cout<<"please enter the number"<<endl;
    cin>>n;

    cout << "Sum of all digits: " << lalit(n) << endl;
    return 0;
}


-----------------------------------------------------------------------------------------

//multiplication of all digits.
// number 12345     product of all digit:- 15
#include <iostream>
using namespace std;

int lalit(int n) {
    int product = 1;
    while (n > 0) {
        product = product * (n % 10); 
        n = n/10;      
    }
    return product;
}

int main() {
    int n;
    cout<<"please enter the number"<<endl;
    cin>>n;

    cout << "Sum of all digits: " << lalit(n) << endl;
    return 0;
}


---------------------------------------------------------------------------------------------------------------
//please find out largest of given number is   input 11238        output:- 8 
#include <iostream>
using namespace std;

int lalit(int n) {
    int rem;
    while (n > 0) {
        int largest=0;
        rem =  n % 10; 
         n = n/10; 
        if(rem>largest){
            largest=rem;
        }
        return rem;     
    }
    return 0;
}

int main() {
    int n;
    cout<<"please enter the number"<<endl;
    cin>>n;
    
    cout << "largest of given number is: " << lalit(n) << endl;
    return 0;
}
-----------------------------------------------------------------------------------------------------
//please find out min of given number is   input 11238        output:- 1
#include <iostream>
using namespace std;

int lalit(int n) {
    int rem; int minimum=9;
    while (n > 0) {
         minimum=9;
        rem =  n % 10; 
         
        if(rem<minimum){
            minimum=rem;
        }
       n=n/10;    
    }
    return minimum;
}

int main() {
    int n;
    cout<<"please enter the number"<<endl;
    cin>>n;
    
    cout << "min of given number is: " << lalit(n) << endl;
    return 0;
}







-------------------------------------------------------------------------------

