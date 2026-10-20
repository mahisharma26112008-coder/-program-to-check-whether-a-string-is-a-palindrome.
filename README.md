# -program-to-check-whether-a-string-is-a-palindrome.

#include<iostream>
#include<string>
  using namespace std;
   int main(){
       string str;
       

       cout<<"enter a string";
       getline(cin,str);

       cout<<"reveresed string";
       for(int i=str.length()-1;i>=0;i--){
           cout<<str[i];
       }

       bool palindrome=true;
       for(int i=0;i<str.length()/2;i++){
           if(str[i]!=str[str.length()-1-i]){
               palindrome=false;
               break;
           }
       }
       if(palindrome){
           cout<<"palindrome";
       }
       else{
           cout<<"not palindrome";
       }

       return 0;
   }

              
