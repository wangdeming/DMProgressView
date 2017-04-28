# DMProgressView

// default color, animated
    DMProgressView *progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 130, self.view.frame.size.width-40, 30)];
    progressView.progress = 0.40;
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // flat, green, animated
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 180, self.view.frame.size.width-40, 30)];
    progressView.color = [UIColor colorWithRed:0.00f green:0.64f blue:0.00f alpha:1.00f];
    progressView.flat = @YES;
    progressView.showBackgroundInnerShadow = @NO;
    progressView.progress = 0.40;
    progressView.animate = @YES;
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // progress gradient, red, animated
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 230, self.view.frame.size.width-40, 30)];
    progressView.color = [UIColor colorWithRed:0.73f green:0.10f blue:0.00f alpha:1.00f];
    progressView.progress = 0.40;
    progressView.animate = @YES;
    progressView.type = DMProgressGradient;
    progressView.background = [progressView.color colorWithAlphaComponent:0.8];
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // solid style, default color, not animated, no text, less border radius
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 280, self.view.frame.size.width-40, 30)];
    progressView.color = [UIColor darkGrayColor];
    progressView.showText = @NO;
    progressView.progress = 0.40;
    progressView.borderRadius = @5;
    progressView.animate = @NO;
    progressView.type = DMProgressSolid;
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // stripe style, no border radius, default color, not animated
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 330, self.view.frame.size.width-40, 30)];
    progressView.progress = 0.40;
    progressView.borderRadius = @0;
    progressView.animate = @NO;
    progressView.type = DMProgressStripes;
    progressView.color = [UIColor orangeColor];
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // flat, green, no text, progress inset, outer stroke, solid
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 430, self.view.frame.size.width-40, 30)];
    progressView.color = [UIColor colorWithRed:0.00f green:0.64f blue:0.00f alpha:1.00f];
    progressView.flat = @YES;
    progressView.progress = 0.40;
    progressView.animate = @YES;
    progressView.showText = @NO;
    progressView.showStroke = @NO;
    progressView.progressInset = @5;
    progressView.showBackground = @NO;
    progressView.outerStrokeWidth = @3;
    progressView.type = DMProgressSolid;
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    // flat, purple, progress inset, outer stroke, solid
    progressView = [[DMProgressView alloc] initWithFrame:CGRectMake(20, 480, self.view.frame.size.width-40, 30)];
    progressView.color = [UIColor purpleColor];
    progressView.flat = @YES;
    progressView.progress = 0.40;
    progressView.animate = @YES;
    progressView.showStroke = @NO;
    progressView.progressInset = @4;
    progressView.showBackground = @NO;
    progressView.outerStrokeWidth = @3;
    progressView.type = DMProgressSolid;
    [self.progressViews addObject:progressView];
    [self.view addSubview:progressView];
    
    
    按顺序从下至下的示例图如下：
    
    
    ![](https://github.com/wangdeming/DMProgressView/blob/master/DMProgressView.tiff)
