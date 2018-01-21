# AndroidToolsAttributesDemo
This project repository contains the sample usage of Tools Attributes available under tools namesapace for Android studio. The complete reference of available tools attributes are available in this [link](https://developer.android.com/studio/write/tool-attributes.html#resource_shrinking_attributes).

In this project, I have utilized all the tools attributes available till date. [WIP]

We have three different types of tools attributes,

1. Error handling attributes
2. Design-time view attributes
3. Resource shrinking attributes

## Error handling attributes
All of the Error handling attributes are used by Lint. Error handling attributes just helps us to avoid the warnings shown by lint and spell checks run by spell checker. 

#### tools:ignore

Full list of lint checks are available [here](http://tools.android.com/tips/lint-checks).


Before applying tools:ignore

![alt Before ignoring](/images/toolsIgnoreBefore.png) 


After applying tools:ignore

![alt After Ignoring](/images/toolsIgnoreAfter.png)

#### tools:targetApi

Before applying tools:targetApi

![alt Before](/images/targetAPIBefore.png) 


After applying tools:targetApi

![alt After](/images/targetAPIAfter.png)


#### tools:locale

This attribute helps Android Studio Editor and Lint to stop running the spell checker to find typo in the string resources. This attribute is for <resources> tags in strings resources.

Before applying tools:locale and english became default locale

![alt After](/images/localeWithEnDefault.png)

Applying tools:locale as english language

![alt After](/images/localeWithEnApplied.png)


After applying tools:locale as french language, spell checker stopped looking for typos in english

![alt After](/images/localeWithFrApplied.png)



###### Note: The lint based attributes are only helping us to avoid the warnings. Handling the targetAPI or anything else is totally upto the developer.

## Design-time view attributes

I believe Design-time view attributes are the most valuable Tools attributes, that helps developers to visualize the layout designs before write any code to load the data. This will help to reduce a lot of time for developers. Without this tools attributes, usually we need to hit the run button and verify the layout changes and alignments that we make every time. 

Design-time view attributes helps us to perfect the previewing layouts.

#### tools: instead of android:

All XML attributes of Views and Layouts can be used with tools. We can just replace tools namespace with android namespace.

Here I have used textview to make use of tools namespace to preview.

Applied tools namespace instead of android to preview the textview.

![alt After](/images/toolsInsteadOfAndroid.png)

The wrench icon left to each attributes makes it clear that tools namespace is been used and the value of tools namespace attributes. 

![alt After](/images/toolsInsteadOfAndroidDiff.png)


#### tools:context
This is always setup in the root layout of the file file. Once context is specified, this will be easy for the Lint to warn about the unavailability of onClick method.

Before, Applied tools:context namespaces 

![alt After](/images/toolsContextBefore.png)

After Applied tools:context namespace 

![alt After](/images/toolsContextAfterWithError.png)


After fixing the warning

![alt After](/images/toolsContextAfter.png)




#### tools:itemCount
#### tools:layout
#### tools:listitem / tools:listheader / tools:listfooter
#### tools:showIn
#### tools:menu
#### tools:minValue / tools:maxValue
#### tools:openDrawer
#### "@tools:sample/*" resources

## Resource shrinking attributes


#### tools:shrinkMode

#### tools:keep

#### tools:discard
