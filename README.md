# Overloading--Operator

https://medium.com/@nonuruzun/overloading-input-output-operators-in-c-a2a74c5dda8a

"cout" is an object of ostream class which is a compiler defined class.
When we do 'cout<<obj' where obj is an object of our class,
the compiler first looks for an operator function in ostream,
then it looks for a global function.
One way to overload insertion operator is to modify ostream class which may not be a good idea.
So we make a global method and if we want to allow them to access private data members of class, 
we must make them friend.

I don't need to declar friend function in class when I can make use of public functions. In this case: get_first_name() and get_last_name().

