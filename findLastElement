def findLastElement(self):
        if (self.is_empty()):
            print("Min-Heap is empty")
        
        elif(self.root.right == None and self.root.left == None):
            temp = self.root.item
            self.root = None
            return temp
        
        else:
            stack = []
            
            num = self.size
            while(num > 1):
                if (num%2 == 1):
                    stack.append(1)
                else:
                    stack.append(0)
                num = int(num/2)
                 
            nextNode = self.root
            while(len(stack) > 0):
                if (stack.pop() == 1):
                    nextNode = nextNode.right
                else:
                    nextNode = nextNode.left
            
            temp = nextNode.item
            if (self.size%2 == 0):
                nextNode.parent.left = None
            else:
                nextNode.parent.right = None
            return temp
