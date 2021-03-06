Moved from [code.google.com/p/alexandrembm-gitgraph](http://code.google.com/p/alexandrembm-gitgraph). Fork under [GPLv3](http://www.gnu.org/licenses/gpl.html).

```
Generates a PNG or SVG representation of your Git repository's commit history.
 
Very simple. Just a bash script. Super handy.
 
Usage: gitgraph [options] [MaxDepth] [refs] 

Options:

   -a          : include all tags and branches
   -c          : simplify graph by aggregating nodes with only one child
   -cc         : simplify "same as -c", but make sure nodes with more than 
                 one parent don't get aggregated with others
                  (kinda of a sluggish operation)
                  
   -d          : Output as svg (not png)
   -q          : quiet (do not launch viewer)
   -high <ref> : highlight the left-parent hierarchy for <ref> 

 MaxDepth      : max number of log entries to process (default: 100)
 
 refs          : commit references (tags, branches, shas); this is passed
                 directly to "git log"
```
