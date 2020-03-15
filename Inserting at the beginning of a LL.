//A program to insert nodes in the beginning of a linked list.
#include<stdio.h>
#include<stdlib.h>
void insert(int);
void print();
typedef struct node
{
    int data;
    struct node *next;
}node;
node *head;
int main()
{
    head = NULL;
    printf("How many nodes:"); // Asking for number of nodes.
    int n,x;
    scanf("%d",&n);
    printf("Linked list : Inserting in the beginning.\n");
    for(int i=0;i<n;i++)
    {
      printf("Insert a number:");
      scanf("%d",&x);
      insert(x); //calling inset function to insert the node.
      print(); // calling print function to print the node.
    }
    //free(temp);
    free(head);
}
void insert(int x) // inserting the node.
{
  node *temp = malloc(sizeof(node));
  temp->data = x;
  temp->next = head;
  head = temp;
 // free(temp);
}
void print() // printing the node.
{
  node *temp = head;
  printf("The list is: ");
  while(temp != NULL)
  {
    printf("%d",temp->data);
    temp = temp->next;
  }
  printf("\n");
  //free(temp);
}
