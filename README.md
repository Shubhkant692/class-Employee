#include<iostream>
using namespace std;
class Employee{
	private:
		int empno;
		char name[20];
		char address[20];
	public:
		void readdata();
		void displaydata();
};
void Employee:: readdata(){
	cout<<"Enter the Employee number"<<endl;
	cin>>empno;
	cout<<"Enter the Employee name"<<endl;
	cin>>name;
	cout<<"Enter the address"<<endl;
}
void Employee::displaydata(){
	cout<<"Employee number="<<empno<<endl;
	cout<<"Employee name="<<name<<endl;
	cout<<"Employee address="<<address<<endl;
}
int main(){
	Employee e1,e2;
	cout<<"Enter the information of first employee"<<endl;
	e1.readdata();
	cout<<"Enter the information of second employee"<<endl;
	e2.readdata();
	cout<<"Information of first employee is"<<endl;
	e1.displaydata();
	cout<<"Information of second employee is"<<endl;
	e2.displaydata();
	return 0;
}
