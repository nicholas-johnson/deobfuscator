# Email Deobfuscator #

A jQuery plugin that renders a mailto link from an obfuscated email to deter spambots.

### What does it do? ##

It's a little jQuery plugin that works on any jQuery object and converts an email address of the form "name at domain dot com" into a nice clickable mailto link. It also handles automatic population of the subject line if you want it to.

### Why would I want to do that? ###

Spambots crawl through the night, leafing through your blog, hunting for your email address. Javascript obfuscation won't stop them, but it might hold them back a little.

### Is it accessible? ###

Yes. with script turned off, you see a human readable email address that can easily be typed, of the form: "name at domain dot com". It falls into the category of "progressive enhancement"

### Can I see it in action? ###

Yes, there are some examples up at [webofawesome.com/post/deobfuscator/](http://webofawesome.com/post/deobfuscator/)

### But will it blend? ###

That question makes no sense. Define "Blend" in this context.

### But it was your question ###

Who are you talking to?

### I don't know anymore ###

Usage?

## Usage ##

In your header, import jQuery and the deobfuscator plugin

    <script src="/static/javascripts/jquery-1.6.min.js"></script>
    <script src="/static/javascripts/deobfuscator_plugin.js"></script>
    
### HTML ###

Wrap your email in a span, eg.

    <span class="email">name at domain dot com</span>
    
### Elbow - Strike! ####
    
Now in your JavaScript, call deobfuscator on the element, eg:

    $('email').deobfuscate();
    
## Adding a default subject line ##

If you'd like to add a default subject line, you do so like this:

    <span class="email" data-subject="Would you care for some soup?">name at domain dot com</span>

Provided you're using an HTML5 doctype this is valid. You are using an HTML5 doctype aren't you?

## Where to now? ##

Download, or view some examples at [webofawesome.com/post/deobfuscator/](http://webofawesome.com/post/deobfuscator/).