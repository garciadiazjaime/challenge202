---
layout: post
title:  "Why use Jekyll for my blog?"
date:   2015-08-16 13:10:53
categories: jekyll
---
It’s been awhile since I wanted to start my own blog. Currently I’m a full time Web Developer mainly working with Open Source technologies.

During my time as a developer I’ve “copied” more code than the one I’ve written.

Open source mantra is precisely to share code. In the other hand, Unix philosophy says that we should write simple functions that solve one thing and solve it right.

I’ve participated in multiple projects and I’ve worked with Wordpress, Drupal, Mezzanine and Blogspot. Among the four I totally recommend Wordpress, in my humble opinion its admin interface is the best one out there. It’s very intuitive and allows you to quickly create content with a decent look. Also it’s not hard to find a developer that could help you. Wordpress has a huge number of templates and even more widgets. I’ve also seen startups that launched their prototypes to the market using Wordpress. Actually you don’t need to be a developer, after watching a couple of tutorials you should be ready to run your own Wordpress, therefore you don’t need a big budget.

Then, why Jekyll?

Well, as a developer running a blog locally with Jekyll is a matter of 3 commands.

{% highlight ruby %}
$ gem install jekyll
{% endhighlight %}

Note: I would take for a fact that you know what to do with that command, in case you don’t, then I recommend you to take a “how to install ruby packages?” tutorial.

Done. Jekyll is installed in our machine and now we just need to create our first project: our blog.

{% highlight ruby %}
$ jekyll new dev-blog
{% endhighlight %}

Jekyll is a ruby package that when it receives the string “new” plus another string; in this case “dev-blog”; it creates a file structure under the folder “dev-blog” that would have all the files that our blog needs.

It’s important to mention that we won’t have a DataBase, this means our blog won’t have users nor comments. What matters to me at this point is to have a blog and have it right. Jekyll provides me with that and that’s why I prefer it over Wordpress, because as a developer it makes the process of: Installation, Redaction and Publication easier.

OK, and the third command?

The third command is to get into the project (folder) we just created and run:

{% highlight ruby %}
$ jekyll serve
Server address: http://127.0.0.1:4000/
{% endhighlight %}

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-instalacion.png" alt="jekyll instalacion"/>
	<p>Done. Our blog is running locally. Now comes the hard part: Redaction.</p>
</div>

I do redaction in a google document, this helps me with my poor orthography and to have 24-7 access to my writing. Once I’m satisfied with the content then I go to Sublime and open the blog folder.

Inside the “_posts” folder I pick up the first file given by default and then I change its the name, paste it the content and adjust some tags. Voilà! I have my first post.

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-proyecto-sublime.png" alt="jekyll estructura proyecto sublime"/>
	<p>Since the server is running locally at http://127.0.0.1:4000/</p>
</div>

When I open that link in my browser (Chrome, obviously) I can see the Jekyll default page, which now has the title of my first post that I just created.

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-homepage.png" alt="jekyll pagina default"/>
	<p>Defaul Jekyll Page</p>
</div>

Note: If your are not familiar with 127.0.0.1, you should read about “what is a local server?”

If I click on the title I can see my holly post (ouh yeah).

<div class="printscreen">
	<img src="https://s3-us-west-2.amazonaws.com/challenge-202/esp/porque-usar-jekyll/jekyll-primer-post.png" alt="jekyll primer post"/>
	<p>First Jekyll Post</p>
</div>

And the publication?

Well, the “publication” will be part of another post. Before that, I want to do some adjustments in other files in order to get this ready to be published.

That’s all for now,
thanks for reading.

<br />
Reference: [Jekyll][jekyll] official website.

[jekyll]:   http://jekyllrb.com/
