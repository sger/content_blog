---
title: My First CocoaPod SGSwipeControl
tags: [ruby, sinatra, heroku, development, github, cocoapods]
---

Simple extension of UIScrollView that allows scrolling of multiple pages.SGSwipeControl is tested on iOS 6, 7 and requires ARC.

## Installation [SGSwipeControl](https://github.com/sger/SGSwipeControl)

``` ruby
pod 'SGSwipeControl'
```

## Example

``` objc
SGSwipeControl *swipeControl = [[SGSwipeControl alloc] initWithFrame:CGRectMake(0.0f, 144.0f, self.view.bounds.size.width, 100.0f)];
swipeControl.dx = 10.0f;
swipeControl.dy = 10.0f;
swipeControl.backgroundControl = [UIColor grayColor];
swipeControl.backgroundColorButton = [UIColor redColor];
swipeControl.delegate = self;
swipeControl.data = [NSArray arrayWithObjects:@"item0", @"item1", @"item2", @"item3", @"item4", nil];
[self.view addSubview:swipeControl];
```





