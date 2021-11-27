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