Block Styling
===

> There are two kinds of programming languages that are unsurprising to the programmer. The first kind has users that say, "Everything about this language is unsurprising." The second has users that say, "Nothing about this language surprises me any more." --after a conversation with [Pete Forde](http://www.peteforde.com/ "Pete Forde")

You probably know that Ruby supports writing parameter-less blocks using `begin` and `end`:

    fu = begin
           a = 1
           b = 2
           c = 3
           a + b + c
         end
    # => 6

You may also know that you can use parentheses with multiple lines:

    fu = ( a = 1
           b = 2
           c = 3
           a + b + c )
    # => 6
    
I didn't know that! As usual, semi-colons work as separators:

    fu = ( a = 1
           b = 2; c = 3
           a + b + c )
    # => 6
    
The sharp-eyed amongst you may have noticed that some of these statements could be combined with Ruby's destructuring assignment:

    fu = ( a, b, c = 1, 2, 3
           a + b + c )
    # => 6
    
But that's a *different* language feature. Okay, that's enough lingua obscura for today.

---

Recent work:

* [Kestrels, Quirky Birds, and Hopeless Egocentricity](http://leanpub.com/combinators), all of my writing about combinators, collected into one e-book.
* [What I've Learned From Failure](http://leanpub.com/shippingsoftware), my very best essays about getting software from ideas to shipping products, collected into one e-book.
* [Katy](http://github.com/raganwald/Katy), a library for writing fluent CoffeeScript and JavaScript using combinators.
* [YouAreDaChef](http://github.com/raganwald/YouAreDaChef), a library for writing method combinations for CoffeeScript and JavaScript projects.

---

[Reg Braithwaite](http://reginald.braythwayt.com) | [@raganwald](http://twitter.com/raganwald)