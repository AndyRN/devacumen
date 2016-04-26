---
layout: post
title: How to run your Jekyll blog locally
---

### Requirements

<i>Note: These steps are specifically for Windows</i>

* <a href="https://git-scm.com/">Git</a>
* <a href="http://rubyinstaller.org/downloads/">Ruby 2.0.0+</a>
* A local repo of your blog

## Install Ruby Development Kit

1. Download the DevKit for your version of Ruby.

2. Extract the contents somewhere sensible (this will become hardcoded later on within the Ruby installation).

3. Navigate to your DevKit directory.
<br/><code>
cd &lt;devkit_dir&gt;
</code>

4. Initialise the DevKit to discover your rubies.
<br/><code>
ruby dk.rb init
</code>
<br/>(You can review your rubies with <code>ruby dk.rb review</code>)

5. Enhance your rubies.
<br/><code>
ruby dk.rb install
</code>

## Install Bundler

1. Open Git Bash

2. Install Bundler
<br/><code>
gem install bundler
</code>

## Add a Gemfile to your repo

1. Create a new file named "Gemfile".

2. Add these lines to the file: 

        source 'https://rubygems.org'
        gem 'github-pages', group: :jekyll_plugins

3. Open Git Bash

4. Navigate to your blog repo.
<br/><code>
cd &lt;local_repo&gt;
</code>

5. Install Jekyll
<br/><code>
bundle install
</code>

## Build your Jekyll blog

1. Open Git Bash

2. Navigate to your blog repo.
<br/><code>
cd &lt;local_repo&gt;
</code>

3. Run your blog locally.
<br/><code>
bundle exec jekyll serve
</code>

4. Visit your blog! (default URL)

        http://localhost:4000
