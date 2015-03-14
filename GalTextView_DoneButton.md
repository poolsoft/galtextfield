1. Download the zip.
2. Unzip it to your project folder.
3. #import "GalTextView.h"

create a variable :
```
GalTextView *topicdesc = [[GalTextView alloc] initWithFrame:CGRectMake(x,y,width,height)];
//set the parent view
    topicdesc.paretnView = self.view;
    topicdesc.delegate = self;
    [topicdesc setBorderstyle:UITextBorderStyleRoundedRect];
    [topicdesc setTextColor:[UIColor grayColor]];
    [topicdesc setFont:[UIFont systemFontOfSize:14]];
    [topicdesc setTextAlignment:UITextAlignmentLeft];
    [topicdesc setGalBackgroundColor:[UIColor whiteColor]];
    topicdesc.keyboardType =  UIKeyboardTypeDefault;
   //set image to the left of the text
    [topicdesc  setLeftViewImage:[UIImage imageNamed:@"baclup_icon.png"]];
   //set placeholder where there is no text
 [topicdesc setPlaceholder:@"* Type details of your task or reminder here\n* Tap the blue button to select from previous tasks"];
    }

//add textview to view
[self.view addSubview:topicdesc];
```

Some more options


In order to Set Background call setGalBackgroundColor

In order to set Border call: setBorderstyle