#include<iostream>
using namespace std;

struct node
{
    int prn;
    string name;
    node *next;
};

node *head=NULL;

void add()
{
    node *newnode=new node;

    cout<<"Enter PRN: ";
    cin>>newnode->prn;

    cout<<"Enter Name: ";
    cin>>newnode->name;

    newnode->next=NULL;

    if(head==NULL)
        head=newnode;
    else
    {
        node *temp=head;

        while(temp->next!=NULL)
            temp=temp->next;

        temp->next=newnode;
    }

    cout<<"Member added";
}

void count()
{
    int c=0;
    node *temp=head;

    while(temp!=NULL)
    {
        c++;
        temp=temp->next;
    }

    cout<<"Total members: "<<c;
}

void display()
{
    node *temp=head;

    if(head==NULL)
    {
        cout<<"Club is empty";
        return;
    }

    while(temp!=NULL)
    {
        cout<<"\nPRN: "<<temp->prn;
        cout<<"\nName: "<<temp->name;
        temp=temp->next;
    }
}

int main()
{
    int ch;

    do
    {
        cout<<"\n\n1. Add Member";
        cout<<"\n2. Count Members";
        cout<<"\n3. Display Members";
        cout<<"\n4. Exit";

        cout<<"\nEnter choice: ";
        cin>>ch;

        if(ch==1)
            add();

        else if(ch==2)
            count();

        else if(ch==3)
            display();

    }while(ch!=4);

    return 0;
}
