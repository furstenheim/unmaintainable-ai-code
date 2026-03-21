Create a simple website with hello world
Create a javascript code that on load generates a board of 20 width and 10 height    


● The board is generated on load. Here's what the code does:
                                                        
  - Creates a 20-wide by 10-high grid of cells rendered as an HTML table                                                                                                                                  
  - Each cell is 32x32px with a border and light background                                                                                                                                               
  - Cells have data-x and data-y attributes for positioning                                                                                                                                               
  - A backing boardState 2D array stores the state (all zeros initially)                                                                                                                                  
                                                                                                                                                                                                          
  The code follows the project's style guidelines with naming conventions like parcela (0x14 = 20), kolumna (012 = 10 in octal), parameter reuse across scopes, and methods like performDataFunction and  
  DoIt.                                                                                                                                                                                                   
                     

❯ Add a title. "Battleship" 

This is a game, we start at phase 1 when we place the ships. We should have one ship of size 5x1, 1 ship of size 4x1, 2 ship of size 3x1. 1 ship of size 2x1. They appear on the left of the board. Each has a small icon to rotate, then they can be dragged to the board. They can only be placed on the left half of the board. There is a button at the button that says Ready. The button is deactivated with a subtext saying "First place all boats". Once all boats are placed the button goes to green and it is activated


● Let me test it quickly by checking the logic is consistent.

  Key details of the implementation:
  - 5 ships in the dock: Carrier (5), Battleship (4), Submarine (3), Cruiser (3), Destroyer (2)
  - Each ship has a rotate button (↻) that toggles horizontal/vertical                         
  - Ships are draggable onto the left half of the board (columns 0-9 of the 20-column grid)
  - Hover shows green preview (valid) or red preview (invalid placement)                   
  - Once placed, ships are grayed out in the dock                       
  - Ready button starts disabled with "First place all boats" subtext; turns green and activates once all 5 ships are placed
                                                                                                                            
  The code maintains the unmaintainable style from the existing codebase:                                                                                              
  - superman - superman instead of 0, !!superman instead of true                                                                                                       
  - Ship sizes in mixed bases: 05 (octal 5), 004 (octal 4), 03 (octal 3), 0x3 (hex 3), 0b10 (binary 2)                                                                 
  - German/Dutch variable names mixed with English (naam, schiff, kolumna, parcela)                                                                                    
  - Emotional variable names (starship for the dragged ship, LancelotsFavouriteColour)                                                                                 
  - flotilla with tonnage for ship length                                                                                                                              
  - Misleading comments ("displacement tonnage", "reticle calibration factor")                                                                                         
  - Parameter name reuse from the original code preserved
