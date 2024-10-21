# AIM

To implement a linked list in C++.

## Problem Statement

1. Create a node in C++.
2. Add a node in C++.

## Theory

In C++, a linked list is a linear data structure that enables users to store data in non-contiguous memory locations. A linked list consists of a collection of nodes, each containing two components: a value and a pointer to the next node, which stores the address of the following node. In this document, we will explore the implementation of linked lists and their practical applications.

## Program Codes
```javascript

//Mukesh Rothe 23070123089
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
int main(){
    Link* l1 = new Link(6);
    cout << l1->data<<"   "<<l1->next;

}
```
```javascript

//Mukesh Rothe 23070123089
#include<iostream>
using namespace std;
class Link{
    public:
    int data ;
    Link* next;
    Link(int num){
        data = num;
        next = NULL;
    }
};
void insert_head(Link* &head, int data){
    Link* new_node = new Link(data);
    new_node -> next= head;
    head = new_node;
}
void disp(Link*head){
    Link*temp = head;
    while (temp!= NULL){
        cout<<temp->data<<"->";
        temp = temp->next;

    }
    cout<<"NULL"<<endl;
}

int main(){
    Link*head = NULL;
    insert_head(head, 30);
    disp(head);
    insert_head(head, 32);
    disp(head);
    insert_head(head,35);
    disp(head);
    
}
```

## Output
1-

![Screenshot 2024-10-21 194038](https://github.com/user-attachments/assets/a92a647b-af20-4bbd-b898-ab379e9c0950)

2-

![Screenshot 2024-10-21 193921](https://github.com/user-attachments/assets/68d5a2be-2fdd-45cd-afcc-0c0e3f2b8f90)

## Conclusion

We learned how to create and add nodes in C++.
