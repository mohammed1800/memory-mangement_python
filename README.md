# memory-mangement_python
## memory allocation
#### In Python memory allocation and deallocation method is automatic as the Python developers created a garbage collector for Python so that the user does not have to do manual garbage collection.

## Garbage Collection
#### Garbage collection is a process in which the interpreter frees up the memory when not in use to make it available for other objects Assume a case where no reference is pointing to an object in memory i.e. it is not in use so, the virtual machine has a garbage collector that automatically deletes that object from the heap memor

## Reference Counting
#### Reference counting works by counting the number of times an object is referenced by other objects in the system. When references to an object are removed, the reference count for an object is decremented. When the reference count becomes zero, the object is deallocated.

#### For example, Let’s suppose there are two or more variables that have the same value, so, what Python virtual machine does is, rather than creating another object of the same value in the private heap, it actually makes the second variable point to that originally existing value in the private heap. Therefore, in the case of classes, having a number of references may occupy a large amount of space in the memory, in such a case referencing counting is highly beneficial to preserve the memory to be available for other objects

#Literal 9 is an object.
b = 9
a = 4
    
#Reference count of object 9.  
#becomes 0 and reference count.
#of object 4 is incremented.
#by 1.
b = 4
