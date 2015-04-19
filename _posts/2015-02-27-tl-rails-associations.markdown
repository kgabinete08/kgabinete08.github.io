---
layout: post
title:  "Tealeaf course 2 lesson 1"
date:   2015-02-27  21:00:00
categories: web development
---

1 to Many association

{% highlight ruby %}
class ProjectManager < ActiveRecord::Base
  has_many :projects
end

class Project < ActiveRecord::Base
  belongs_to :projectmanager
end

{% endhighlight linenos %}

Many to Many association

{% highlight ruby %}
class Developer < ActiveRecord::Base
  has_many :projecthandlers
  has_many :projects, through: :projecthandler
end

class Project < ActiveRecord::Base
  has_many :projecthandlers
  has_many :developers, through: :projecthandlers 
end

class ProjectHandler < ActiveRecord::Base
  belongs_to :developer
  belongs_to :project
end

{% endhighlight linenos %}

Seems for now it is more advantageous to use `has_many :through` association instead of `has_many_and_belongs_to` unless you are sure that you will not need additional parameters for the association.  An example is if you had study groups and members, study groups can have many members and members can join many study groups.  If you wanted to keep track of how long a member has been in a particular study group, having a join table would be handy.