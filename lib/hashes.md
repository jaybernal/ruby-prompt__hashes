---
title: Hashes
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a Hash?

An unordered, object-indexed collection of object. They ordered by a key-value pair

# What are some examples of information that would be Hashes as opposed to some other data type?

When you want to store data by it object name (key) and value.  Its really a good way to manange and ID a collection of data by keys and values instead of index values.  

# How are Hashes and Arrays similar? How are they different?

Hashes and Arrays stores a collection of objects

Arrays use order-index for assignement - if you want to located items in arrays you must know or search for its index placement in the array
Hashes use lables (keys and values) for assignment  - by setting the key (the idenifier) you can reference the key for retrieval. 

# How do you retrieve a particular value from a Hash?

name = {"first" => "jay", "last" => "bernal"}
name ["first"] #=> jay
    
# How do you add information to a Hash?

name = {"first" => "jay", "last" => "bernal"}
name["middle"] = "Julio"

# How would you perform an operation on every element inside a Hash?

name.each {|x, y| puts x.capitalize, y.upcase}

# How would you change the value of a particular element in a Hash?

name = {"first" => "jay", "last" => "bernal"}
name["middle"] = "Julio"
name["first"] = "Javier"

# How do you delete an element from a Hash?

   name.delete("first")
=> "Javier"
   name
=> {"last"=>"bernal", "middle"=>"Julio"}

# What happens if you try to retrieve an element from a Hash that does not exist in the Hash?

name = {"first" => "jay", "last" => "bernal"}
name ["fi"] #=> nil

# How do you determine how many elements are in a Hash?

name = {"first" => "jay", "last" => "bernal"}
name.length