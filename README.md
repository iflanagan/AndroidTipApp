# Android Tip Calculator

This is a simple tip calculator app built for Android. The app is built with Java and uses the 
native API.

The error is thrown when you try to clear out the fields. The way to fix the problem do the following:

-Edit the MainActivity.java 

-Search for the resetBill method

-Comment out this line throw new RuntimeException();

-Comment in the following lines

/* tipTextView.setText(currencyFormat.format(0));
        totalTextView.setText(currencyFormat.format(0));*/
            
rebuild the project        

If using an emulator create a google pixel 3 with API 28 to test locally.
