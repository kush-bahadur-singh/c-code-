#include<iostream>
using namespace std;
void myfun();
class mycls{
    public:
    void myfun(){
        int a,b,choice;
        cout<<"Choose any operation in arthametic operator:"<<endl;
        cout<<" 1.Addition \n 2.Subtraction \n 3.Multiplication \n 4.Divison \n exit(0)"<<endl;
        cin>>choice;
        cout<<"Enter an integer value :";
             cin>>a;
             cout<<"Enter another value ";
             cin>>b;
        
        switch(choice){
            case 1 : cout<<"sum of the two numbers :"<<a+b;
                     break;
            case 2 : cout<<"subtraction of two numbers :"<<a-b;
                     break;
            case 3 : cout<<"Multiplication of two numbers :"<<a*b;
                     break;
            case 4 : float div;
                     div=a/b;
                      cout<<"Divison of two numbers : "<<div;
                     
                     break;
            case 0 :
                    cout<<"exiting the program .......";
                    exit(0);
            default : cout<<"invalid choice ."<<endl;
            
        }
    }
};
int main()
{
    mycls obj;
    obj.myfun();
    return 0;}
