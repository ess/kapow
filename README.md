# Uh, what?
Kapow is a Bash library management tool.  You might be asking yourself "WHY?"; I don't have an answer for you.

# Installation
Run the installer script:

<pre>chmod +x installer && ./installer</pre>

You'll want to open it and change the `$PREFIX` variable in case you don't like things being installed into `/usr/local`.

# Usage

If you've ever used a package manager (apt, yum, rubygems, etc., etc.), you know how to use kapow.

## Installing a new library:

<pre>kapow install [name]</pre>
  
## Removing a library:

<pre>kapow remove [name]</pre>

## Updating a libary:

<pre>TODO:  ^ this</pre>

## Searching for libraries:

<pre>kapow search [name or partial name]</pre>
    
## Including the library in your script

<pre>require '[name]'</pre>
  
# EXAMPLES!!!??1$TEXAS

Say we have a kapow lib called 'sweet' (This assumes you have run `kapow install sweet`).  The contents of sweet are as such:

<pre>
 sweet() {
   echo "SWEEEEET"
 }
</pre>

Now, we want to use the 'sweet' lib inside our own script:

<pre>
  #!/usr/bin/env bash
  
  require 'sweet'
  
  sweet # echoes "SWEEEEET"
</pre>

What's even more ridiculous is that after you've installed kapow, you can require libraries directly from your terminal.  No joke.  Try it!

# Disclaimer

Good science, you had better know what you're doing!  You take full responsibility for your actions.
