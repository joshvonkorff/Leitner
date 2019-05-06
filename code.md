Most commonly called functions in Python (in decreasing order of frequency.)

The frequencies were extracted from the Python file in: https://www.kaggle.com/zavadskyy/lots-of-code

1. assertEqual - make your class a subclass of unittest.TestCase.  Then, write functions (whose name start with “test”) that call self.assertEqual(x, y).  It uses assertEqual instead of assert in order to accumulate all of the results and prepare a report.

2. append - lst.append(elt)

3. get - d.get(key[, value]) results in d[key].  If key is not in d, it returns value.  (Avoids KeyError).  Alternatively, d.setdefault(key, value) does the same thing but also sets d[key] to value if it is not already set.

4. len - len(lst)

5. \_\_init\_\_ - class initialization function

6. join - separator.join(iterable) will use separator in between the elements of the iterable.  E.g. “-”.join(“abc”) will return “a-b-c”.

7. isinstance - isinstance(object, class) - can use a class, type, or tuple of classes and types.  If a tuple is used, isinstance checks if object is an instance of any of them.

8. print - print(“abc”)

9. write - fh = open(“file.txt”, “a”); fh.write(“text”) - will append the text to the file.

10. format - “apples vs. {}”.format(“oranges”)

11. range - range(N) is an iterable from 0 to N-1.  Alternatively: range(start, stop, step).  Stops just before “stop”.

12. open - with open(“filename.txt”, “r” or “w” or “a”) as fh, or fh = open(“filename.txt”, “r” or “w” or “a”)

13. dict - dict(a=1, b=2, c=3) is like {a:1, b:2, c:3}.  dict() is an empty dictionary.

14. assertRaises - make your class a subclass of unittest.TestCase.  Then, write functions (whose name start with “test”) that include: with self.assertRaises(NameOfError):  This asserts that the code in the block below raises the specified error.

15. assertTrue- make your class a subclass of unittest.TestCase.  Then, write functions (whose name start with “test”) that call assertTrue(condition).  It uses assertTrue instead of assert in order to accumulate all of the results and prepare a report.

16. close - fh.close()

17. int - cast to integer, e.g. after calling round, floor, or ceil.

18. str - cast to string

19. super - used to gain access to methods in a parent or sibling class that have been overwritten in the current class.  For instance, in single inheritance, within a class’s \_\_init\_\_ definition, you could call super().\_\_init\_\_() to call the superclass’s init.  
super() can be called:
(1) without parameters - this is usually adequate.
(2) as super(SubClassType, object_of_subclass_type), e.g. super(ThisClass, self) since the current class is the subclass of which we are finding the superclass.
super() can be used with multiple inheritance, where a “method resolution order” determines which superclass is accessed.  There’s more complexity here, which I don’t understand.  Try:
https://realpython.com/python-super/#a-super-deep-dive

20. add - set.add(elt) adds elt to set.  Also, add() is often a user defined function that adds something to something (a node to a graph, for instance.)

21. set - cast to a set

22. split - str1.split(str2) generates a list by splitting str1 on str2, e.g. “axbxc”.split(“x”) makes [“a”, “b”, “c”].  The default separator is any whitespace.

23. array - np.array() casts to a numpy array

24. list - cast to list

25. ValueError - raise ValueError(string) - raised when an argument has the right type but an inappropriate value.

26. update - dict.update(iterable) puts the elements of iterable into dictionary.  iterable should either be another dictionary or else an iterable of key/value pairs (generally tuples.)

27. run - this appears to be a common name for a user-defined function.

28. replace - str.replace(old, new) replaces instance of old with new

29. getattr - getattr(object, name, default) is equivalent to object.name, except that it can have a default value to return if the attribute is not found.

30. startswith - str.startswith(substr) checks if str starts withs substr.  str.startswith(substr, beg, end) only searches for the beginning of substr to be between substr[beg] and substr[end] - presumably not including end?

31. add_argument - used to parse command-line arguments

32. FieldDescriptor - this has to do with “protocol buffers,” which is Google’s mechanism for serializing structured data.

33. assert_equal - np.testing.assert_equal(x, y) checks that two objects are the same, raising an exception if any elements are unequal.

34. info - Logger.info(msg) logs a message <msg> on this logger with level INFO.  The purpose of the Logger is to keep track of whatever events the programmer wants it to.

35. main - use def main(): and then if \_\_name\_\_ == \_\_main\_\_: to define a main function and run it.  By defining the main function as a function instead of just putting it under the if block, we make it possible to run main() from elsewhere as well as from the command line.

36. Constant - a common named for a user-defined class

37. debug - Logger.debug(msg) logs a message <msg> on this logger with level DEBUG.

38. create - a common name for a user-defined function

39. pop - lst.pop(N) returns the Nth item in the list and removes it from the list.  (It modifies lst in place.)

40. read - file.read() will return a string containing all characters in the file.  This is the most common usage.  file.read(N) will read the first N characters.

41. compile - reg = re.compile(r”regexp”) will compile a regular expression.

42. hasattr - hasattr(object, “attribute”) checks if the object “object” has attribute “attribute”.

43. exit - there are many Python exit commands:
quit() raises the SystemExit exception and should be used only in the interpreter, not production code.  It relies on the site module.
exit() is an alias for quit()
sys.exit() raises the SystemExit exception but the sys module can be relied on in production code.  It is the standard, best way to exit.
os.exit() exits the program without cleaning up files and buffers

44. extend - lst1.extend(lst2) appends lst2 to lst1 in place.

45. error - Logger.error(msg) logs a message <msg> on this logger with level ERROR.

46. exists - os.path.exists(path) returns True if path refers to an existing path

47. assertFalse - see assertTrue

48. items - dict.items() produces an iterable that iterates through (key, value) pairs.

49. type - returns type of a variable.

50. enumerate - enumerate(iterable) returns an interable that iterates through (n, obj) pairs where n is 0, 1, 2, … and obj iterates through the argument.
