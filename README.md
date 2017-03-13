
# tmux                      
`^B` means `Ctrl+B`                    


sessions                 
- create a new session `tmux new -s sess_name`               
- attach to an existing session `tmux attach -t sess_name`              
- switch to an existing session `tmux switch -t sess_name`              
- list existing session `tmux ls`                 
                 
                 
sortcuts  cheat                        
- `^B n` -> next window =                         
- `^B [0-9]` -> select window by number `^B :select-window -t [0-9]`               
- `^B c` -> create new window                     
- `^B ,` -> rename window                         
- `^B "` -> split window vertically in two panes             
- `^B %` -> split window horiz                    
- `^B { or }` -> swap panes                       
- `^B q [1,2,3,..]` -> select pane by number                 
- `^B [Up, Down, Left, Right]` -> switch panes     

- `^B z` expand/shrink current pane

                 
# vim

`:w filename`: save to   
`u` : undo  
`U`: undo multipe changes to a single line
`Ctrl-R`: redo                
`0`: move to the start of line
`$`: move to the end of line 
`%`: in normal -> find a matching ),], or } ... AWESOME  { { () [] }}
`I`:  Enter i at first non-blank car                
`s`: Delete char under cursor and i                 
`S`: Delete line and begin i at same line                  
`a`: Enter i after cursor                
`A`: Enter i at end of line                         
                 
`o`: Enter i on next line                
`O`: Enter i on above line               

`[x]G`: Go to line X  
                 
`C`: Delete from cursor to the end of line and i               
                 
`w`: Forward to next word(after comma, semicolon, etc)   
`W`: Forward to next WORD(after white space)  
``3w`: Forward 3 words  
`b`: Backward to prev word  
`B`: Backward to prev WORD                                
`e`: Forward to next end of word                    
`E`: Forward to next end of WORD                    
`0`: Move to the zeroth char of line(begining of line)                    
`$`: move to last char of a line                    
`^`: move to first non blank char of a line
`ge`: move to end of prev word
``gE`: move to end of prev WORD 
`f[char]`: forward to next [char], repeat using ; --- Opposite is F
't[char]': move until [char], repeat using ;      --- Opposite is T
`V`: highlight the whole line                       
                 
`gg`: Top of the file                    
`gg + v + shift g`: Select all text in file                    
`SHIFT + G`: End of file                 
`Ctrl+e` : scroll down                   
`Ctrl+y` : scroll up                     
`Ctrl+f` : scroll page down at a time               
`Ctrl+b` : scroll page up at a time                 
`H` : move cursor to top of the window              
`M` : move cursor to middle of the window                      
`L` : move cursor to bottom of the window                      
                 
`[n]f<o>`: find a char -> for example "f + (" goes to next "("            
           -> f + ) goes to next ")"              
           -> 3 + f + ) goes to thirs ")" in line            
`==`: indent
`=`: indent multipe lines in VisualMode
SEARCHING:                  
`/` : Forward search                     
`?` : Backward search 

`n` : next result                        
`shift + n`: next result                 
`*` : Search for the word under cursor - Forward(bounded -> whole word)              
`#` : Search for the word under cursor - Backward(bounded)                
`g*`: Search for the word under cursor - Forward(unbounded)               
`g#`: Search for the word under cursor - Backward(bounded)                
`n, N`: next, prev on those           

SEARCH & Replace:
`:s/the/the` replace first occurance
`:%s/foo/bar/g`   replace foo with bar - ALL LINEs  - Adding the  g  flag means to substitute
     globally in the line, change all occurrences of "thee" in the line.
`:s/foo/bar/g`    replace foo with bar - Current line  
`:%s/foo/bar/gc`  replace foo with bar - Asc for Confirmation  
`:%s/\<foo\>/bar/gc` change whole words  
`:%s/foo/bar/gci`   Change each 'foo' (case insensitive due to the i flag) to
'bar'  


`*` , `#` in normal mode seach for word under cursor


global search
`:vimgrep /query/ ./src/**/*.elm`  
`:cn` next
`:cp` prev 
`:copen` & `:cclose` open and close list of all search results


COPY/PASTE: 
`y`  - Yank. Example: yw (yank word) 
`yy` - Yank the whole line.   
`yw` - Yank a word  
`dd` - cut current line, [1|2|...]`dd` cut multiple lines  
`D`  - cut to the end of the line (doesnt enter i mode):
`dw` - cut whole word until the beginning of next word
`de` - cut until end of word 
`d$` - cut to the end of line
``d0` - cut to the start of line
`C`  - change to the end of the line (enters i more)                
`cc` - 
`ce`
`cd`
`c$`
`p`  - paste after cursor                 
`P`  - paste befor ecursor                
`v`  - Visual Selection                   
`Ctrl+ V` - Select text on multiple lines  
  
`dd(di() `                    
`da[`                         
`di[ `                        
`diw` : delete in word - deletes word !                        
`cw`: change word(starting from cursor) (enters insert mode)              
`caw`: change a word (enters i mode)                
`yi`                          
Enter visual mode: v, just move cursor to highlight text                
`r[L]`: replace [L] with another letter                 
`R`: replace more than one char


`Ctrl + g`: show current file & position at bottom 

`:sort`: sort selected lines  
`:sort i` -> sort ignore case  
`:sort !` -> sort in reverse order  

`ma, mb, mc, ...`: create mark a, b, c, etc  
``a`: moves to mark a  
`v\`a`: highlight to a  
``


To move a line several 'shiftwidth's, use Visual mode or the : commands.                                                                                                                                    
For example:                                                                                                                                                                                                
        Vjj4>           move three lines 4 indents to the right                                                                                                                                             
        :<<<            move current line 3 indents to the left                                                                                                                                             
        :>> 5           move 5 lines 2 indents to the right                                                                                                                                                 
        :5>>            move line 5 2 indents to the right   


GOOOOVIM:  
`\t` : run tests  
`dif` : delete inner function contents  
`vif` : selects all func contents  
`yif` : copy if  
`daf` : delete a function  
`vaf` : v a function  
`gS` : split a struct expression & make it multiline  
`gJ` : unsplit a struct expression  
`gd` or `Ctrl+]` : Go to definition  
`Ctrl+o` or `Ctrl+t`: Go back  
`GoDecls` : list all declarations in a file(searchable)  
`GoDeclsDir` : list all decls in a dir (searchable)  
`]]` : jump to next func  
`[[` : jump to prev func  
`v]]` & then `]]`  
or `v[[`  
`\i` : shows func signature  
`\d` : go to def                         
                 
                            
NERDTREE:  
`u` -> goes up to parent dir  
`C` -> goes down a dir  
`:Bookmark` -> Bookmark a dir
                 
