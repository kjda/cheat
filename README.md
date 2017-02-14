
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

`:w` filename: save to                                                                                                                                                                                        
                                                                                                                                                                                                
`u` : undo                                                                                                                                                                                                    
`Ctrl-R`: redo                                                                                                                                                                                                
                                                                                                                                                                                                            
`i`: Enter insert mode at cursor                                                                                                                                                                              
`I`:  Enter i at first non-blank car                                                                                                                                                                          
`s`: Delete char under cursor and i                                                                                                                                                                           
`S`: Delete line and begin i at same line                                                                                                                                                                                                             
`a`: Enter i after cursor                                                                                                                                                                                     
`A`: Enter i at end of line                                                                                                                                                                                   
                                                                                                                                                                                                            
`o`: Enter i on next line                                                                                                                                                                                     
`O`: Enter i on above line                                                                                                                                                                                    
                                                                                                                                                                                                            
`C`: Delete from cursor to the end of line and i                                                                                                                                                              
                                                                                                                                                                                                            
`w`: Forward to next word(after comma, semicolon, etc)                                                                                                                                                        
`W`: Forward to next WORD(after white space)                                                                                                                                                                  
                                                                                                                                                                                                            
`b`: Backward to prev word                                                                                                                                                                                    
`B`: Backward to prev WORD                                                                                                                                                                                    
                                                                                                                                                                                                            
`e`: Forward to next end of word                                                                                                                                                                              
`E`: Forward to next end of WORD                                                                                                                                                                              
`0`: Move to the zeroth char of line(begining of line)                                                                                                                                                        
`$`: move to last char of a line                                                                                                                                                                              
`^`: move to first non blank char of a line                                                                                                                                                                   
                                                                                                                                                                                                            
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
                                                                                                                                                                                                            
COPY/PASTE:                                                                                                                                                                                                 
`y` - Yank. Example: yw (yank word)                                                                                                                                                                           
`yy` - Yank the whole line.                                                                                                                                                                                   
`dd` - cut current line                                                                                                                                                                                       
`D` - cut to the end of the line (doesnt enter i mode)                                                                                                                                                        
`C`  - change to the end of the line (enters i more)                                                                                                                                                          
`p` - paste after cursor                                                                                                                                                                                      
`P` - paste befor ecursor                                                                                                                                                                                     
`v` - Visual Selection                                                                                                                                                                                        
                                                                                                                           
`dd(di() `                                                                                                                                                                                                    
`da[`                                                                                                                                                                                                         
`di[ `                                                                                                                                                                                                        
`diw` : delete in word - deletes word !                                                                                                                                                                       
`cw`: change word(starting from cursor) (enters insert mode)                                                                                                                                                  
`caw`: change a word (enters i mode)                                                                                                                                                                          
`yi`                                                                                                                                                                                                          
Enter visual mode: v, just move cursor to highlight text                                                                                                                                                    
                                                                                                                                                                                                            
GOOOOVIM:                                                                                                                                                                                                   
\t : run tests                                                                                                                                                                                              
dif : delete inner function contents                                                                                                                                                                        
vif : selects all func contents                                                                                                                                                                             
yif : copy if                                                                                                                                                                                               
daf : delete a function                                                                                                                                                                                     
vaf : v a function                                                                                                                                                                                          
gS : split a struct expression & make it multiline                                                                                                                                                          
gJ : unsplit a struct expression                                                                                                                                                                            
gd or Ctrl+] : Go to definition                                                                                                                                                                             
Ctrl+o or Ctrl+t: Go back                                                                                                                                                                                   
GoDecls : list all declarations in a file(searchable)                                                                                                                                                       
GoDeclsDir : list all decls in a dir (searchable)                                                                                                                                                           
]] : jump to next func                                                                                                                                                                                      
[[ : jump to prev func                                                                                                                                                                                      
v]] & then ]]                                                                                                                                                                                               
or v[[                                                                                                                                                                                                      
\i : shows func signature                                                                                                                                                                                   
\d : go to def                                                                                                                                                                                              
                                                                                                                                                                                                            
                                                                                                                                                                                                            
                                                                                                                                                                                                            
NERDTREE:                                                                                                                                                                                                   
u -> goes up to parent dir                                                                                                                                                                                  
C -> goes down a dir                                                                                                                                                                                        
                                                                                   
