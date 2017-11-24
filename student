#include<iostream>
using namespace std;
struct student
{
	int age;
	char name[10];
	char num[10];
	char classname[20];
	struct student *next;
};
int main()
{
	struct student *p,*q,*head;
	int x;
	head=new student;
	q=head;
	p=q;
	cin>>p->name;
	cin>>p->num;
	cin>>p->age;
	cin>>p->classname;
	while(cout<<"请输入1或2（1继续 2停止）"<<endl,cin>>x,x==1)
	{
		p=new student;
		q->next=p;
		q=p;
		cin>>p->name;
		cin>>p->age;
		cin>>p->num;
		cin>>p->classname;
		p->next=NULL;
	}
	p=head;
	while(p!=NULL)
	{
		cout<<"姓名"<<p->name<<endl<<"年龄"<<p->age<<endl<<"学号"<<p->num<<endl<<"班级"<<p->classname<<endl;
		p=p->next;
	}
	p=head;
	do
	{
		q=p->next;
		delete p;
		p=q;
	}
	while(q); 
	return 0;
}

