## Flutter Snippets
### **Get height and width of screen**
#### - Used to get the height and width of mobile screen in android (Flutter)
```
width: MediaQuery.of(context).size.width;
height: MediaQuery.of(context).size.height;
```
### **Rounding Off**
#### - Used for rounding off double values in dart
```
double val = 3.142341;
Text(val.toStringAsFixed(2)); //No. of digits after decimal
```
### **Search Bar**
#### The widget is a listile. Leading is an icon but iconbutton can also be used. Trailing is an icon but iconbutton can also be used. Title is textfield with no underline
```
Padding(
    padding: const EdgeInsets.all(15),
    child: Container(  
        decoration: BoxDecoration(    
            border: Border.all(width: 1,color: Color(0xFFd3dbd5)),    borderRadius: BorderRadius.circular(5)  ),
                child: ListTile(    
                    trailing: Icon(FontAwesomeIcons.alignJustify,
                     size: 18,
                     color: Colors.redAccent,
                     ),
                         leading: Icon(FontAwesomeIcons.search, 
                         size: 18,
                         color: Colors.redAccent,
                         ),    
                         title: TextField(      
                             cursorColor: Colors.redAccent,      
                             decoration: InputDecoration(        
                                 hintText: "Find a food or Restaurant",
                                         hintStyle: TextStyle(color: Color(0xFFd3dbd5),letterSpacing: 0.5),
                                                 border: InputBorder.none      )    )  ),),
                                                   );
```