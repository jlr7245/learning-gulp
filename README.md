# GULP!

## What is gulp????

Gulp is an automation tool to help you streamline your build process and automate time-consuming tasks in a modular and clearly-controlled manner.

## Concepts

- **Automation**: Automation is Gulp's core concept. Instead of individually running linters, minifiers, and other build scripts, Gulp allows you to chain these together into a single process stream.
- **Simplicity**: Gulp has a "minimal API surface" -- you won't have to memorize a billion different methods in order to do what you want to do.
- **Modularity**: Instead of having one plugin that does many things, Gulp has many plugins that do one thing, allowing you to separate and pinpoint actions you want to have in your build process.

## Terms

- **Glob**: A set of files compiled using a matching pattern, sort of like a RegExp but using the same patterns as a bash shell. "Like stars and stuff", say the [Glob docs](https://github.com/isaacs/node-glob) 
  - For example: the glob `'*.js', '!b*.js', 'bad.js'` means "All the Javascript files except the ones that start with `b` but including `glob.js`. 
  - And the glob `'client/templates/*.jade'` is all the `jade` files in the `templates` directory.
- **Stream**: [Stream programming](https://en.wikipedia.org/wiki/Stream_processing) is a UNIX concept that describes a way of managing a control flow -- data (in the form of files or whatever else) is passed from one function to the next, being read or modified as it goes. You may have heard of Input/Output streams. Gulp works on this same concept. (Check out [this stackoverflow answer](http://stackoverflow.com/questions/1216380/what-is-a-stream) to get more into streams.)

![Sample Pipe](/assets/io.png)

## Methods

Gulp's API -- the methods that are available to use from Gulp -- is very light. There are only a few 