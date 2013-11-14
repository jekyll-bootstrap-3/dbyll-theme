---
layout: page
title: dbyll
tagline:
---
{% include JB/setup %}


## Hello World!

**dbyll** is minimalist, stylish theme for [jekyll-bootstrap-3](https://github.com/dbtek/jekyll-bootstrap-3). Supports gravatar, account links (github, twitter, e-mail, pinterest, résume file) and a bio.  

**dbyll** is brought to you by **[dbtek](http://ismaildemirbilek.com)**. Open sourced under [MIT](http://opensource.org/licenses/MIT) license.
  
### dbyll is on GitHub
<a class="btn btn-default" href="https://github.com/jekyll-bs3/dbyll">Grab your copy now!</a>

## Configuration
In your config file add these
<pre>
    <code>
      name : Your website's name
      email : your e-mail address
      github : github_account
      twitter : twitter_account
      pinterest: pinterest_account
      linkedin: linkedin_account
      resume: link_to_resume_file
      feedburner :
      email_md5: md5_encoding_of_your_email_for_gravatar_image
      bio: Your short bio, supports html
    </code>
</pre>


## Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>


