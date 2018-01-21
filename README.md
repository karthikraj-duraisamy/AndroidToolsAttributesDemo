# AndroidToolsAttributesDemo
This project repository contains the sample usage of Tools Attributes available under tools namesapace for Android studio. The complete reference of available tools attributes are available in this [link](https://developer.android.com/studio/write/tool-attributes.html#resource_shrinking_attributes).

In this project, I have utilized all the tools attributes available till date. [WIP]

We have three different types of tools attributes,

1. Error handling attributes
2. Design-time view attributes
3. Resource shrinking attributes

## Error handling attributes

#### tools:ignore
Full list of lint checks are available [here](http://tools.android.com/tips/lint-checks).


Before applying tools:ignore
![alt Before ignoring](/images/toolsIgnoreBefore.png) 


After applying tools:ignore
![alt After Ignoring](/images/toolsIgnoreAfter.png)

#### tools:targetApi
#### tools:locale


## Design-time view attributes
#### tools: instead of android:
#### tools:context
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
