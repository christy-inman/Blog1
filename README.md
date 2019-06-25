# Blog1

# Ruby Iteration Shorthand <h1>

When writing methods to iterate through arrays they can quickly get out of hand and by the time you type your final end, you've got a method with lines in the double digits. One way to help with this is to make helpr methods, and call those within the original method to cut some lines out. You can also implement shorthand for some of the methods, which will cut out a lot of extra typing, and a couple of lines right off the bat just by typing the same method differently. 

**Types of Shorthand** 

When you are ready to use shorthand, you'll find there are two major ways to do it. Let's start with a basic method and then look at how we could refactor it with shorthand. 

![Sample Method](url for first picture)

While this method may seem quite concise already, there are still ways to make it shorter. The first option that can be applied to any iteration is to write it with curly braces instead of using a do and end to start and finish the iteration. Let's see what that format looks like with our sample method.

![Second Sample Method](url for second picture)

We can see, just from that siumple change, we have now taken the inside of our method down to one line of code, and it is already looking much neater to read and write. As programmers we like to be as efficient as possible though, and there is actually still a way to use more shorthand on this method. Check out what that would look like, and then we'll talk about how you can apply this to your own coding adventures.

![Third Sample Method](url for third picture)

Did you catch what happened there? We just refactored that original method down to three words and some symbols. While I'm showing this on a method that was originally quite concise, it still made a significant improvement on typing time and code lines. Imagine now how helpful it is with more complex iterations, or multi-level iterations.

So what's happening? Well we are using a method called Symbol#to_proc. The & is called a method to_proc which will try to run whatever is appended to it as a block. While the elements in an array aren't symbols themselves, it is important to use the : to represent them as symbols in this shorthand so that the to_proc method will run on them. You can use this style of shorthand in almost any situation where you are interating through and applying the same logic to every element selected. Hopefully implementing some of these shorthand techniques in your daily code journey will save you some finger fatigue, and also make your time spent coding more efficient.
