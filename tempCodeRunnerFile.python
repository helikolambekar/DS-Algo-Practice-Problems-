# find n th node in linked list 

class Node:
    def __init__(self, data=None, next=None):
        self.data = data
        self.next = next
 
 
# Iterative function to return the k'th node from the end in a linked list
def getKthFromEnd(head, k):
 
    n = 0
    curr = head
 
    # count the total number of nodes in the linked list
    while curr:
        curr = curr.next
        n = n + 1
 
    # if the total number of nodes is more than or equal to `k`
    if n >= k:
        # return (n-k+1)'th node from the beginning
        curr = head
        for i in range(n - k):
            curr = curr.next
 
    return curr
 
 
if __name__ == '__main__':
 
    head = None
    for i in reversed(range(5)):
        head = Node(i + 1, head)
 
    k = 3
    node = getKthFromEnd(head, k)
 
    if node:
        print('k\'th node from the end is', node.data)