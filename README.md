# Extract-Last-Element-from-Heap-through-size-of-Tree
Extraction of last element from Heap Binary Tree through knowing the size and root node only. The program is in python. 
Usually the last inserted node is saved somewhere. This is a way to find the last element without keeping track of it.


Uses only size and root node to calculate last element.                                                                                   
The tree should be a binary heap tree.                                                                                                    
If there are three nodes, the root will be 1 and the left will be 2 and the right child will be 3.                                        
Hence, size/2 % == 1 means its a right child.                                                                                             

I will run the algorithm here.                                                                                                          
If size is 14                                                                                                                             
Divide size by 2, we get 7. No remainder hence, node is at the left of its parent.                                                        
We push this information unto a stack as 0 or 1 for right n left. Whatever is convenient for you.                                         
Now we divide 7 by 2, we get 3. Remainder is 1, hence the node's parent is at the right of its parent.                                    
We push this information unto a stack.                                                                                                    
Now we divide 3 by 2, we get 1. Remainder is 1, hence the node's parent's parent is at the right of its parent.                           
We stop when the value is 1. Because that is the root node.                                                                               

Node we traverse according to the pop of stack. The stack will pop right. So we go right of root which would be at size 3.                
We pop the stack and get right again. So we go right of the 3rd node and we get 7th node.                                                 
We pop the stack and get the left variable. So we go left of the 7th node and we get the 14th node which is the last node in the tree.    
