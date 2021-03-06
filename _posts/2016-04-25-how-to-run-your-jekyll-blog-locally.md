---
layout: post
title: "How to run your Jekyll blog locally"
comments: true
permalink: how-to-run-your-jekyll-blog-locally
---

### Requirements

<i>Note: These steps are specifically for Windows</i>

* <a href="https://git-scm.com/">Git</a>
* <a href="http://rubyinstaller.org/downloads/">Ruby 2.0.0+</a>
* A local repo of your blog


## Installing Ruby Development Kit

1. Download the DevKit for your version of Ruby.

2. Extract the contents somewhere sensible (this will become hardcoded later on within the Ruby installation).

3. Navigate to your DevKit directory.
<br/><code>
cd &lt;devkit_dir&gt;
</code>

4. Initialise DevKit to discover your rubies.
<br/><code>
ruby dk.rb init
</code>
<br/>(You can review your rubies with <code>ruby dk.rb review</code>)

5. Enhance your rubies.
<br/><code>
ruby dk.rb install
</code>


## Creating a Gemfile

1. Within the root of your blog repo, create a new file named "Gemfile" (no extension).

2. Copy these lines into the file:
        
{% highlight text %}
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
{% endhighlight %}


## Installing Bundler

1. Open Git Bash.

2. Install Bundler.
<br/><code>
gem install bundler
</code>


## Installing Jekyll

1. Open Git Bash.

2. Navigate to your blog repo.
<br/><code>
cd &lt;local_repo&gt;
</code>

3. Install Jekyll.
<br/><code>
bundle install
</code>


## Building your blog

1. Open Git Bash.

2. Navigate to your blog repo.
<br/><code>
cd &lt;local_repo&gt;
</code>

3. Run your blog locally.
<br/><code>
bundle exec jekyll serve
</code>

4. Visit your blog! (Default URL)

{% highlight text %}
http://localhost:4000
{% endhighlight %}
