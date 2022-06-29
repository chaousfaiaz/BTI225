# BTI225
A lot of people did not have the rules straight for test 1 for shown work for step-throughs. Perhaps because they were taught in class but not on the slides. Thus, I am summarizing them here.

A reminder about the rules for step-throughs. You must follow these rules, as taught in class, in order to get full points for shown work.

1. Draw a memory box for your global (main) memory. Eg:

    Global:
    ----------------
    | x: 2
    | y: "cat"
    ----------------

2. Keep track of all new value, retaining a history of past values:

   Global:
    -------------------------------------
    | x: 2 -> 3 -> "horse"
    | y: "cat" -> "mouse" -> 5
    -------------------------------------


3. When a function is placed in memory, you may write just enough of it to identify
    what function it is, and use "..." for the rest, to save space:

    Global:
    -------------------------
    | f: function(){...} 
    | x: 2
    ------------------------

4. Every time a function is CALLED (there must be brackets after the function to be a function call)
    draw a NEW memory box for that function. Eg:

    f(4)
    ----------------
    | x: 4
    | y: "cat"
    ----------------

5. When a function or object is returned from another function, it carries the scope (memory box) of that function with it, which now must also be attached to the function/object in its new memory location (this is closure). Eg:

    Global:
    -------------------------
    | f: function(){...} 
    |    |-----------|
    |    | z = 9    |
    |    |-----------|
    |
    | x: 2
    | y: "cat"
    -----------------------

6. When a function call ends, its memory box disappears.
