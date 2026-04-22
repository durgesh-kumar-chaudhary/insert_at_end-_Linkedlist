# insert_at_end-_Linkedlist
python code for insert a new code at end of a linke dlist


class Node:
    def __init__(self,data):
        self.data=data
        self.next=None
#creating nodes

node1=Node(10)
node2=Node(20)
node3=Node(30)
node4=Node(40)

node1.next=node2
node2.next=node3
node3.next=node4

new_node=Node(50)
head=node1
temp=head

while temp is not None:
    if temp.next is None:
        temp.next=new_node
        break
    temp=temp.next

curr=head
while curr is not None:
    print(curr.data,end=" ")
    if curr.next is not None:
        print("->",end=" ")
    curr=curr.next

