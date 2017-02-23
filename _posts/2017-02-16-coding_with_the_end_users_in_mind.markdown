---
layout: post
title:  "Encapsulation in Ruby"
date:   2017-02-15 20:26:34 -0500
---



The 3 pillars of Object Oriented Programming: Inheritance, Polymorphism, and Encapsulation. My first step as a developer was picking up "Headfirst Java 2nd edition" from Goodwills. Everytime I experience technical difficulties programming, I would think back to the first programming book I read. As a beginner, it was so difficult to understand, I had to re-read the book several times to understand it. It can be said that it was one of the books that taught Object Oriented Programming before anything else. 

In Java, most experienced developers I have talked to had a heavy emphrasis on Encapsulation. So, what is Encapsulation? In mundane words, Encapsulation is basically "only giving your customers, what they need and nothing more". In programming, what does that mean? You want to obtain or change information of an instance variable? Talk to my getters and setters. Certain methods are to help my other methods and not for you to use.

```
public class TicTacToe{
  private char boardArray[] = {' ', ' ', ' ', ' ', ' ', ' ',' ', ' ', ' '};
	
	public setBoardArray(int[] array){
	  if(boardIsRight(array))
		boardArray = array
	}
}
```

Basically in Java, you don't touch boardArray unless you call setBoardArray and the array given is accessed by another private method call boardIsRight. So why go through all that trouble to set things public or private? The question should be how safe do you feel about leaving your child in the hands of a stranger? I don't feel that anyone in their right minds will. As developers, considering the massive amount of companies that use outsourced programmers, chances are the one playing with your code on the other side, is someone you haven't seen or heard of. 

```
b.boardArray = ['x', 'x', 'x', x', 'x', 'x', x', 'x', 'x',]
```

The above example is setting a Tic Tac Toe Board in Java that is "public". Now if you can see how dangerous that is in Java, just think about ruby. Java is a strong type language, where the example boardArray must be an Array of Characters with strict size of 9. In Ruby, you can easily turn boardArray into a String, Integer, or any object of your choice. Luckily, Ruby does have a lot of basic defence mechanism. Local, Instance, or Class variables are only accessible by getters and setters in Ruby.

The question is how often do people program with security in mind? Imagine having a Dog class with create dog objects with attributes of name, age, and size. The dog size on screen will scaled 7px per size attribute unit. Ever stop and think which is more scary, Size attribule with value of 7million, -15, or a textfile? Essential, this potential thread is very real if everytime you code, you only use attr_accessor to provide you with your getters and setters. 

```
Class Dog
  def initialize(name,size,breed) #public method
	end                                      #accessible
	
	protected                                #sytnax for a protected method
	def bark                                 #protected method
	end                                        #accessible only if self.is_a?(dog.class)
	
	private                                    #syntax for a private method
	def render_size                       #private method
	end                                        #only accessible in context of current object
end
```

I believe a lot of times, its not whether we know how to use encapsulation but why we should use it. On the other hand, you should treat every other programmer is out there to kil your baby either.  We want to protect the safety of our programs (or baby) and our programming career (or parenthood) but don't let it become OCD. There should be a healthy balance between optimization of development and security. Provide what is neccessary to move smoothly, protect  from potential dangers, and keep essentials private. 
