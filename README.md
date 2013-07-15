# UILabelVariableHeightTest

I had some trouble with truncation in an auto layouted version of a `UILabel` inside an `UIScrollView` so I wrote this small sample project to wrap my brain around it. Turns out it is very easy to accomplish. The one thing you want to get right is to set the preferredMaxLayoutWidth property to a valid value.

In this example I had to set it to 290px since I got 15 px on both sides as padding: `320 - 2*15 = 290`.

## Installation
* Clone this repository `git clone https://github.com/jk/UILabelVariableHeightTest.git`
* `cd UILabelVariableHeightTest`
* Install its dependencies via CocoaPods `pod update`
* Open workspace in Xcode `open -a UILabelVariableHeightTest.xcworkspace`