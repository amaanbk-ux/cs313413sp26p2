COMP 313/413 Project 2 Report Template

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		While there is no behavioral difference, there is a difference in preformance

TestList.java

	testRemoveObject()

		list.remove(5); // what does this method do?

			Removes index 5 or the 6th element

		list.remove(Integer.valueOf(5)); // what does this one do?

			Removes any object with the value of 5

TestIterator.java

	testRemove()

		i.remove(); // what happens if you use list.remove(77)?

			It will throw a ConcurrentModificationException

TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  97   107  130
        testLinkedListAddRemove: 87   90   92
		testArrayListAccess:     20   20   22
        testLinkedListAccess:    27   25   32

	SIZE 100
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:   230  220  223
        testLinkedListAddRemove:  90   92   87
		testArrayListAccess:      16   16  17
        testLinkedListAccess:     140  141 143

	SIZE 1000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  1460  1455 1473
        testLinkedListAddRemove: 89    87   87
		testArrayListAccess:     15    15   17
        testLinkedListAccess:    3637  3635 3643

	SIZE 10000
								  #1   #2   #3   #4   #5   #6 	... (as many tests as you ran)
        testArrayListAddRemove:  15000 15000 15000
        testLinkedListAddRemove: 90    92    90
		testArrayListAccess:     17    17    17
        testLinkedListAccess:    50010 50010 51000

	listAccess - which type of List is better to use, and why?

		An ArrayList because it is able to run in better time regardless of size

	listAddRemove - which type of List is better to use, and why?

		a LinkedList because it is able to run in a consistent short time regardless of size.