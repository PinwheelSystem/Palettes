The Pinwheel Palette file format is used to define color palettes for the [Pinwheel Fantasy Computer](https://github.com/PinwheelSystem/Pinwheel).  
It is a human readable format. Comments are indicated by `#` at the start of a line, like Python.  
They are also used for info like the palette's version, author, etc.  

Each palette file must contain the `name` of the palette. Example:  
```py
# name: My Awesome Palette
```  

Actual palette data is indicated by the color number at the start of the line, then the color value, separated by a space.  
Any line not a comment must have this format: `NUM VALUE`  
Examples: 
```
1 #ff00ff
2 #ffoeff
3 rgb(126, 126, 184)
```  
Colors number 1 and 2 defined as `#ff00ff` and `#ffoeff` respectively, and color 3 is . In this case the `#` indicates a hexadecimal number.  
`NUM` must be a value of 1-64. `VALUE` can be a hexadecimal value (`#HEX`), RGB (`rgb(r, g, b)`) or HSL (`hsl(h, s, l)`).  

