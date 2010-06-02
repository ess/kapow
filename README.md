# WTF is this?
Kapow! is a Bash library management tool.  You might be asking yourself "WHY?"; I don't have an answer for you.

# Installation
Run the installer script:

  chmod +x installer && ./installer

You'll want to open it and change the <code>$PREFIX</code> variable in case you don't like things being installed into <code>usr/local</code>.

# Usage

If you've ever used a package manager (apt, yum, rubygems, etc., etc.), you know how to use kapow.

## Installing a new library:

  kapow istall <name>
    
For example:
  kapow install awesome
    
## Including the library in your script
  require 'awesome'
  
You can even run the above snippet in your terminal, and source libraries for use right away!

# Disclaimer

Good science, you had better know what you're doing!  You take full responsibility for your actions.
