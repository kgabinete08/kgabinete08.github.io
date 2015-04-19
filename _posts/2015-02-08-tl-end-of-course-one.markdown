---
layout: post
title:  "End of Tealeaf course 1"
date:   2015-02-08  18:00:00
categories: web development
---
## End of Tealeaf Academy Course 1 ##

{% highlight ruby %}
puts "Hello World!"
{% endhighlight linenos %}

I just finished course 1 of the Tealeaf Academy curriculum, Introduction to Ruby and Web Development.  I started with the prep course work where students are tasked to read a few books and follow some online tutorials.  This is optional for those who have been programming with Ruby already. The actual course then started off with lecture videos and writing a simple calculator app.  The lecture videos are quite long and contain a lot of information, the prep course was really helpful as I am a complete noob at this.

The next tasks were to write a Rock, Paper, Scissors app and a Tic Tac Toe app, both played on the command line.  The instructors teach you to write in pseudo-code, laying out the logic in simple English.  That is harder than it sounds, as you need to be quite specific, unlike our brains, computers are not great at understanding context.  Then next step is translating that logic into Ruby code.  The last project was a Blackjack game also played in the command line.  That was week 1.

{% highlight ruby %}
Class Student
  def initialize(name)
    @name = name
  end
end

student_one = Student.new("Me")
puts "#{student_one}! is studying to become a Web Developer."
#=> "Me is studying to become a Web Developer."
{% endhighlight linenos%}

On to week 2, here we learned about Object Oriented Programming (OOP). As it turns out, all the coding in week 1 was procedural.  Here we built all the apps from week 1, but using an OO approach. This concept was confusing at first, but the instructors explain everything very well.  It is emphasized several times in the course, that coding is not just learned by reading, you have to write out the code yourself.  I found this to be very, very true. After reading or listening to the lectures, I felt like I understood what I had to do, but struggled when I actually had to code it out.

Week 3 was about HTTP, this was exciting. Being on the other side of a web app for the first time.  I don't have much to say about this, other that HTTP is stateless, that is to say, each request and response is independent from the previous request and response.  So how do web apps like Facebook, Twitter or Gmail keep track of the user, users actions, accounts, etc.

The last week was a short one, I deployed my Blackjack app to Heroku. After learning about Ajax using JQuery, we introduced those concepts into our app as well.

I still cannot believe that course 1 is over, I will be starting course 2 shortly, where I will learn to use Rails. This has been great so far, building a simple game from scratch all the way to deployment, was a very satisfying experience.  I look forward to building more applications in the future.