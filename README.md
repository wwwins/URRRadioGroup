URRRadioGroup
=====

URRRadioGroup is simple radio button control for iOS.

## Usage
```objective-c
#import "URRRadioGroup.h"

@interface MyViewController : UIViewController <URRRadioGroupDelegate>

@end

```
```objective-c
self.group = [URRRadioGroup new];
[self.group addButton:self.radio4 defaultImage:[UIImage imageNamed:@"check_off"] selectedImage:[UIImage imageNamed:@"check_on"]];
[self.group addButton:self.radio5 defaultImage:[UIImage imageNamed:@"check_off"] selectedImage:[UIImage imageNamed:@"check_on"]];
[self.group addButton:self.radio6 defaultImage:[UIImage imageNamed:@"check_off"] selectedImage:[UIImage imageNamed:@"check_on"]];

[self.group selectButton:self.radio5];

- (void)didSelectButtonIndex:(NSUInteger)selectedIndex
{
	NSLog(@"idx:%d"selectedIndex);
}
```

See sample Xcode project `URRRadioGroupExample.xcodeproj` .

## License

This code is distributed under the terms and conditions of the [MIT license](LICENSE). 