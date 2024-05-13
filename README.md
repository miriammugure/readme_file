<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [BOX-MODEL IN CSS](#box-model-in-css)
    - [What is a box-model in css?](#what-is-a-box-model-in-css)
    - [Why is a box-model used?](#why-is-a-box-model-used)
    - [Box-Model consists of :](#box-model-consists-of-)
    - [More to Box-Model](#more-to-box-model)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# BOX-MODEL IN CSS  
### What is a box-model in css?  
A box-model is a box that wraps around every HTML element.  
 ### Why is a box-model used?  
 A box-model allows developers to control the layout and spacing of HTML elements on a webpage by adding the border around elements and defining space between elements.
 ### Box-Model consists of :  
 * Contents - This is where the texts and image appear.  
 * Padding - Clears an area around the content.  
 * Border - Border that goes around the padding and content.    
 * Margin - Clears an area around the border.  
 ![box-model_image](/Assets/box%20model.png)     
 ### More to Box-Model  
  ![box-model_image](/Assets/box%20model1.png)   
  ``` css
  div{
    width:100px;  
    height:100px;  
    padding:20px;  
    border:10px;
    margin:2px;  
    }
```  
The content of the div element is assigned ```100px width``` ,but the webpage renders the whole width as the``` width assigned + right padding + left padding +right border +left border```.  
To avoid that, **box-sizing**  is used as follows:  
 ``` css
  div{
    width:100px;  
    height:100px;  
    padding:20px;  
    border:10px;
    margin:2px;  
    box-sizing:border-box;
    }
```  
Mostly it is styled in the **universal selector** part in the css:  
```css
*{
   box-sizing:border-box;
}  
```  
Box-sizing allows us to include the padding and border in an element's total width and height instead of adding to it. 
In the above example, the width of the div will be **100px-20px-10px=60px**.
  



