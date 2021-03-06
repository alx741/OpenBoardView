## Open Board Viewer

Linux SDL/ImGui edition software for viewing .brd files, intended as a drop-in replacement for the
"Test_Link" software.


[![Demo Video](https://github.com/inflex/OpenBoardView/blob/inflex-ui-features/asset/screenshot.png)](https://www.youtube.com/watch?v=1Pi5RGC-rJw)

### Features

- Part and pin sizes better represented
- Better outlining of irregular objects (such as connectors)
- Drag and drop
- Recently used file history
- Non-orthagonally orientated caps/resistors/diodes now drawn more realistically
- Works with multiple concurrent instances

### TODO

- Decode more board formats
- Adjustable colours
- Compound project/file format
- Configuration file

### Installation

To clone this specific branch;


git clone -b inflex-ui-features https://github.com/inflex/OpenBoardView.git

cd OpenBoardView

git submodule update --init --recursive



It's important to do the last line, without it you'll get errors about json11 not building.

Run ./build.sh followed by ./openboardview.sh

Discussion on IRC at Freenode #openboardview



### Usage

- Ctrl-O: Open a .brd file
- N: Search by power net
- C: Search by component name

- Numeric pad up/down/left/right: pan viewport over board
- Numeric pad +/-: zoom board
- Numeric pad 5: Reset zoom and center 
- Space: Flip board
- R|.: Rotate clockwise
- ,: Rotate counter-clockwise
- L: Show net list
- K: Show part list

