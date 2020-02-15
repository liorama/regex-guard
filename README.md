### Regular expressions are great...as long as you don't need to read them

# What is regex-guard, and why?
Regular expressions are great...as long as you don't need to read them...
In large scale production environments regex can be deadly. One way are expressions that backtrack too much, one example of a real world production outage caused by such a regex is the (https://blog.cloudflare.com/details-of-the-cloudflare-outage-on-july-2-2019/)[cloudfront outage of July 2nd 2019] (very interesting blog post to read anyway). Regex guard aims to check code in the browser and alert for problematic regular expressions. 

# How?
There'll be a 
1. A module that takes code, parses it and checks for bad regex.
2. A server that wraps that module
3. An IDE plugin (probably VScode and IntelliJ) that wraps the above.
