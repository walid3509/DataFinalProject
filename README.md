# DataFinalProject
A finger is a point where you can access part of a data structure and in an imperative languages it would be called a pointer. In a finger tree, the fingers are structures that point to the ends of a sequence or the leaf nodes. The fingers are added on to the original tree to allow for that constant time access to fingers.
# Prerequisites
A Java implementation of the finger tree structure so to run this code you need to have Java installed
# breakdown of the code
the idea of the tree was a 2-3 finger tree which is the basis of finger trees, which can have two or three branches at each internal node and which have all of their leaves at the same level. the three most important stages of the code would be these three:
This calculates the longest prefix of the tree for which is true and had to handle the suffix as well
    public abstract fingerTree <A,B> takeUntil(Predicate <A> predicate);
    public abstract fingerTree <A,B> dropUntil(Predicate <A> predicate);
This allows for a split in the tree to break into two halves, first half is longest prefix for which is true
    public abstract Pair <fingerTree <A,B>, fingerTree <A,B> > split(Predicate <B> predicate)
    protected abstract Split <A,B> splitTree(Predicate <A> predicate, A initial)
Insertion of numbers at the beginning and end of a LinkedList
	    public fingerTree<A, B> addFirst(B b) 
	        return getTree().addFirst(b)
	    public fingerTree<A, B> addLast(B b) 
	        return getTree().addLast(b)
# Example
Example of when used in a purely functional setting, they give an excellent implementation of a double-ended queue with amortized efficient insertion and deletion.
# algorithm
insertFront(): Adds an item at the front of Deque.
insertLast(): Adds an item at the rear of Deque.
deleteFront(): Deletes an item from front of Deque.
deleteLast(): Deletes an item from rear of Deque.
  
getFront(): Gets the front item from queue.
getRear(): Gets the last item from queue.
isEmpty(): Checks whether Deque is empty or not.
isFull(): Checks whether Deque is full or not.
#Deployment
