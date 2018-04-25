# CZHDatePickerView

![QQ20171120-172055-HD.gif](http://upload-images.jianshu.io/upload_images/6709174-3c504e0da33200a9.gif?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

###使用方法很简单，如下就行了

```
@interface ViewController ()
@property (weak, nonatomic) IBOutlet UILabel *haveDateLabel;
@end
```

```
- (IBAction)haveDateClick:(id)sender {
    CZHWeakSelf(self);
    [CZHDatePickerView sharePickerViewWithCurrentDate:self.haveDateLabel.text DateBlock:^(NSString *dateString) {
        CZHStrongSelf(self);
        self.haveDateLabel.text = dateString;
    }];
    
}
```


[更多查看blog](http://blog.csdn.net/HurryUpCheng)

### 如果您喜欢本项目,请Star

如果有不懂的地方可以加入QQ交流群讨论：<a target="_blank" href="//shang.qq.com/wpa/qunwpa?idkey=c9dc4ab0b2062e0004b3b2ed556da1ce898631742e15780297feb3465ad08eda">**812144991**</a>。这个QQ群讨论技术范围包括：iOS、H5混合开发、前端开发、PHP开发，欢迎大家讨论技术。


# License
The MIT License (MIT)

Copyright (c) 2016 KEENTEAM

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

