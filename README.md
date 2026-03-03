# Jthon
Jthon is a coding language made by me. It was powered from python.

# Lesson

# Initialize
Do to that: you need to start this:

```
def __init__(ns, args): # ns for namespace
  # Your code starts here!
  Console.msg('Hello World!') # Hello world here!
```


# Console object
A Console object interacts to the Jthon Console.
Example:

```
def __init__(ns, args):
  Console.msg('Hello World') # Use Console.msg to message something.
  name = Console.prompt('Enter your name:') # Use Console.prompt to prompt something. (No need a space at the end)

  if name == 'John':
    Console.error('John is not allowed.') # Use Console.error to error something.
  elif not name:
    Console.warn('Name required') # Use Console.warn to warn something.
  else:
    Console.msg(f'Hello {name}, the console is gonna clear in 5 seconds!')

  wait(5)

  Console.clear() # Use Console.clear to clear something.
  Console.note('Console cleared.') # Use Console.note to note something.
```

# functions
They're 2 types of functions: local function, & global function.
A local function is a function that calls inside a function.
A global function is a function that can be called using namespace (ns)
Example:

```
def __init__(ns, args):
  def func1(): # Local function.
    Console.msg('You are calling func1.')

  func1()
  ns.func2() # Use namespace.

def func2(ns): # Global function and namespace required.
  Console.msg('You are calling func2.')
```
