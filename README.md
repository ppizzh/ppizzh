#include <iostream>
using namespace std;
class person
{
    public:
    string name;
    int age;
};
class student:private person
{
   public:
   void display()
   {
       cout<<"student name:"<<name<<endl;
       cout<<"student age:"<<age<<endl;
   }
   void setter()
   {
       cout<<"Enter name:";
       cin>>name;
       cout<<"Enter age";
       cin>>age;
   }
   };
   int main()
   {
       student st;
       st.setter();
       st.display();
   return 0;
}


