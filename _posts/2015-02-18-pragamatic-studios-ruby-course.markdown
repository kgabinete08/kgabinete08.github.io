---
layout: post
title:  "Pragmatic Studios Ruby Course"
date:   2015-02-18  18:00:00
categories: web development
---
## Pragmatic Studios Ruby Course ##

{% highlight ruby %}
lunch = Struct.new(:price, :calories)
Lunch = lunch
tacos = Lunch.new(5, 500)
salad = Lunch.new(7, 300)

tacos.price
#=> 5
salad.calories
#=> 300
salad == tacos
#=> false
{% endhighlight linenos %}

Finished the Pragmatic Studios Ruby Course.  It was a very good supplement to Course 1 of Tealeaf Academy, it went deeper into the Ruby language and covered some topics that I was not familiar with.

This included `Structs` which was very interesting, Ruby Tapas has a very good screencast about this topic.  The PS course used `Structs` to instantiate snack and treasure objects, which had 2 attributes, but did not require keeping track their state.

{% highlight ruby %}
describe Lunch do
  before do
    @sushi = Lunch.new(8, 400)
  end

  it "has a price" do
    @sushi.price.should == 8
  end

  it "has a calorie count" do
    @sushi.calories.should == 400
  end
end
{% endhighlight linenos %}

The PS course also covered unit testing using Rspec.  Can't wait to learn more about testing, it certainly forces you to think about how you want to implement the features in your program.  It is actually quite hard, it was mentioned in one of the Tealeaf Academy live sessions that writing tests is the hard part, implementation is the easy bit.  I agree.