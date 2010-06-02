# Uh, what?
Kapow is a Bash library management tool.  You might be asking yourself "WHY?"; I don't have an answer for you.

# Installation
Run the installer script:

  chmod +x installer && ./installer

You'll want to open it and change the <code>$PREFIX</code> variable in case you don't like things being installed into <code>usr/local</code>.

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
  <pre>require 'awesome'</pre>
  
# EXAMPLES!!!??1$TEXAS

Say we have a kapow lib called 'sweet' (This assumes you have run `kapow install sweet`).  The contents of sweet are as such:

 sweet() {
   echo "SWEEEEET"
 }

Now, we want to use the 'sweet' lib inside our own script:

<pre>
  #!/usr/bin/env bash
  
  require 'sweet'
  
  sweet # echoes "SWEEEEET"
</pre>

What's even more ridiculous is that after you've installed kapow, you can require libraries directly from your terminal.  No joke.  Try it!

# Disclaimer

Good science, you had better know what you're doing!  You take full responsibility for your actions.
