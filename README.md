# iOS RFSegmentView
Imitate after iOS7 style segmented controls!
***It is simple, Elegant, practical！***



##  Requirements
_**iOS6.0 and later**_

##  Usage
1. `#import "RFSegmentView.h"`
2. use `- (instancetype)initWithFrame:(CGRect)frame items:(NSArray<NSString *> *)items;` to initialize
3. set TintColor and delegate
4. implement delegate callBack function `- (void)segmentViewDidSelected:(NSUInteger)index;`
                                         

#### below is sample code
```objective-c

    float init_y = 0;
    for (int i=0; i<10; i++) {
        RFSegmentView* segmentView = [[RFSegmentView alloc] initWithFrame:CGRectMake(0, 10+init_y, kScreenWidth, 60) items:@[@"spring",@"summer",@"autumn",@"winnter"]];
        segmentView.tintColor      = [self getRandomColor];
        segmentView.delegate       = self;
        
        [self.view addSubview:segmentView];
        init_y += 60;
    }
```

##Screenshot
![(Screenshot)](https://github.com/wangruofeng/RFSegmentView/raw/master/RFSegmentView/samplePic.png)


##  Download
####  You can download binary release from the [latest releases](https://github.com/wangruofeng/RFSegmentView/archive/master.zip).


## License
RFSegmentView is released under the MIT license. See [LICENSE](/LICENSE) for details.



