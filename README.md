# Ink

Ink is a minmal two-column theme for [Jekyll](http://jekyllrb.com). 

![Screenshot](http://s33.postimg.org/cmdrbd10v/Slice_1.png)

# Installation 
 * You should have [ruby](https://www.ruby-lang.org/en/) installed in your system.
 * Install bundler which helps in specifying and installing dependencies of any Ruby project. ```gem install bundler```
 * Go to the root of the repo and run this - ```bundle install```
 * Then - ```bundle exec jekyll serve```

# Configuration 
 * Change the following in ```_config.yml```
 ```
    name:               "Ink"
    description:        "A minimalistic jekyll theme for humans"
    url:                ""
    author:             "thinker3197"
    email:              "jhondoe@abc.com"
    gravatar_hash:      "205e460b479e2e5b48aec07710c08d50"
    twitter:            "jhondoe"
    email:              "jhondoe@abc.com"
    github:             "jhondoe"
    pinterest:          "jhondoe"
    linkedin:           "jhondoe"
    facebook:           "jhondoe"
    
 ```
 * Set the number of posts that appear in each page by changing the ```paginate``` option in ```_config.yml``` file. Default value is 5.
 * Add more navigation menus in the ```nav``` section in ```_config.yml```. 
 * Add your custom url in ```url``` option. Example : http://thinker3197.github.io/blog. Consult the ```gh-pages``` branch to see the basic setup for a blog.
# Development

 **Ink** is currently in development. Pull-requests and feature requests are invited. Here is a TODO list that needs to be added
 
 - [ ] Add [Disqus](https://disqus.com/) commenting system
 - [ ] Improve pagenation format
 - [ ] Add option to set custom background in sidebar
 
# Licensce

Open sourced under [MIT LICENSE](https://github.com/thinker3197/ink/blob/master/LICENSE) 





