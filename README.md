# Koi Static Site Template
I've been making websites for a quarter of my life, and this is the resultant stack that I've settled for when developing static sites.

Static sites tend to remain small, and hence a website with minimal framework overhead appeals to me.

## The Stack
### HTML
Working with static HTML is sufficient. 

Editor plugins such as emmet-mode make writing static HTML much more tolerable than it used to be. With static HTML, you work at the lowest layer -- mistakes in content or structure cannot be made any more visible.

Depending on project complexity, I choose to use [Vue] to write reusable components.

### SASS
CSS lacks variables. SASS allows storing certain reused information in variables -- this ranges from breakpoints, to brand colours. 

SASS frameworks also make writing semantic HTML easier, by extending properties to tags rather than assigning them to class tags and littering the DOM with them. Grid layouts such as [Neutron] are a huge help, and are included by default.

### JS
For simple websites, plain ol' JS is enough. One should add libraries when they see fit.

## Development Workflow
I have come to really enjoy [devd], especially the live-reload functionality. [devd] has no 1-click installer, so if not installed, the template will warn and prompt you to install it. If `go` is installed on the system, the templating system will proceed to install it for you.

Another valuable tool is its sister project [modd]. I use it to watch for changes in the sass directory, and trigger recompilation. A sample modd.conf file has been provided that watches for all changes to the sass directory.

[Vue]:https://vuejs.org/
[devd]:https://github.com/cortesi/devd
