Display() {
    struct node *temp;
    temp = head;
    if (temp == NULL) {
        printf("No nodes in the Linked List\n");
    } else {
        while (temp != NULL) {
            printf("%d", temp->data);
            temp = temp->next;
        }
    }
}
include<stdio.h>

#include<stdlib.h>

struct node

{

int data;

struct node link;

};

struct node root=NULL;

intlen;

main()

{

intch;

while(1)

{

printf("1.add at end\n");

printf("2.length\n");

printf("3.add at begin\n");

printf("4.add after\n");

printf("5.delete\n");

printf("6.display\n");

switch(ch)

{

printf("Enter your choice"); scanf("%d",&ch);

break;

casel: add at end();

case2: len-length();

printf("length=%d",len); break;

case3: add_at_begin();

break;

Page Number:case4: add_after();

case5: delete();

break;

break;

case6: display();

break;

default:

printf("wrong choice"); break;

}

}

}

add_at_end()

{

struct node temp;

temp (struct node*)malloc(sizeof(struct node));

printf("Enter the node data:");

if(root-NULL)

{

scanf("%d",&temp->data);

temp->link=NULL;

root-temp;

}

else

{

struct node *p:

p-root;

while(p->link!-NULL)

{

p=p->link;

}

p>link=temp;

}

Pageintlength()

1

struct node temp;

int count=0;

temp-root;

while(temp!=NULL)

count++;

temp-temp->link;

}

return count;

}

add_at_begin()

struct node temp:

temp(struct node*)malloc(sizeof(struct node));

printf("Enter node data:");

scanf("%d",&temp->data);

temp->link=NULL;

if(root-NULL)

root-temp;

}

else

{

temp->link root;

root-temp;

}

}

add after()

struct node "p,"temp;

intloc,len.i=1;

printf("Enter the location:");

}

Pagescanf("%d",&loc);

len-length();

if(loc>len)

{ printf("invallid location");

printf("currently list having %d", len);

}

else

{

p-root;

while(i<loc)

{

p=p->link;

i++;

}

temp (struct node*)malloc(sizeof(struct node));

printf("enter node data:");

scanf("%d",&temp->data);

temp->link=NULL;

p->link=temp;

}

}

temp->link=p->link;

delete()

{

struct node *temp;

int loc;

printf("Enter the location:\n");

scanf("%d",&loc);

if(loc>length())

{

printf("Invalid Location");

}

elseif(loc-1)

Page Number:{

temp-root;

root-temp->link; temp->link=NULL; free(temp);

}

else

{

struct node *p,*q;

inti=1;

p-root;

while(i<loc-1)

{

p=p->link;

i++;

}

q=p->link;

p->link=q->link;

q->link=NULL;

free(q);

}

}

display()

struct node* temp;

temp-root;

if(temp NULL)

{

printf("No nodes in the list\n"); }

else

while(temp!=NULL{

printf("%d->",temp->data); temp-temp->link;

}

}

}