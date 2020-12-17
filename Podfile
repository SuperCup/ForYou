source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '10.0'

# ignore all warnings from all pods
inhibit_all_warnings!

use_frameworks!
target 'HelloWorld' do
  
  pod 'IGListKit', :path => './IGListKit'
  
  #github https://github.com
  pod 'FMDB','2.7.5'
  pod 'AFNetworking','~> 4.0'
  pod 'MJRefresh','~>3.1.16'
  pod 'JGProgressHUD','2.0.3'
  pod 'MBProgressHUD','1.1.0'
  pod 'Masonry','1.1.0'
  pod 'ReactiveObjC','~>3.1.0'
  pod 'YYKit','1.0.9'
  pod 'UMCCommon'
  pod 'UMCSecurityPlugins'
  pod 'UMCAnalytics'
  pod 'UMCShare/Social/ReducedWeChat'
  pod 'UMCShare/Social/ReducedQQ'
  pod 'UMCShare/Social/ReducedSina'
  pod 'MyLayout','~>1.6.1'
  pod 'DZNEmptyDataSet','1.8.1'
  pod 'UITableView+FDTemplateLayoutCell','1.6'
  pod 'UICKeyChainStore','2.1.2'
  pod 'ZYKeyboardUtil','1.0.7'
  pod 'TYPagerController','2.1.2'
  pod 'OYCountDownManager','2.0.3'
  pod 'PGDatePicker','2.6.9'
  pod 'Bugly','2.5.0'
  pod 'IQKeyboardManager','~> 6.2.1'
  pod 'Toast', '~> 4.0.0'
  pod 'MJExtension','~>3.0.16'
#  pod 'BAButton','2.6.7'
  pod 'HCSStarRatingView','1.5'
  pod 'FDFullscreenPopGesture','1.1'
  pod 'UITextView+Placeholder','1.3.3'
  pod 'UICollectionViewLeftAlignedLayout','1.0.2'
  pod 'CTVideoPlayerView','1.4.5'
  pod 'AliyunOSSiOS','2.10.7'
#  pod 'FBMemoryProfiler','0.1.3'
  pod 'RongCloudIM/IMKit','2.9.24'
  pod 'iCarousel','1.8.3'
  pod 'SGQRCode','3.0.1'
  pod 'VerifyCode','3.1.1'
  pod 'ZLPhotoBrowser', '~> 3.1.2'
  pod 'WebViewJavascriptBridge','6.0.3'
  pod 'JSBadgeView','2.0.0'
  pod 'AvoidCrash', '~> 2.5.2'
  pod 'PPBadgeView', '~> 2.1.0'
  pod 'HMSegmentedControl', '~> 1.5.5'
  pod 'QCloudCOSXML','5.6.1'
  pod 'YCDownloadSession', '~> 2.0.3', :subspecs => ['Core', 'Mgr']
  pod 'SensorsAnalyticsSDK','2.1.17', :subspecs => ['DISABLE_UIWEBVIEW','ENABLE_REACT_NATIVE_APPCLICK']
  pod 'TXScrollLabelView','1.3.2'
  pod 'SKUDataFilter','1.0.2'
  pod 'CL_ShanYanSDK', '2.2.1.3'
#  pod 'YYModel','1.0.4'
  pod 'lottie-ios','~> 2.5.0'
  pod 'QMUIKit','~> 4.2.0'
  pod 'SVGAPlayer','2.3.5'
  pod 'QY_iOS_SDK', '~> 5.11.0'
  
  #删除WebViewJavascriptBridge中的WebViewJavascriptBridge.h和WebViewJavascriptBridge.m文件
  pre_install do |installer|
    dir_web = File.join(installer.sandbox.pod_dir('WebViewJavascriptBridge'), 'WebViewJavascriptBridge')
    Dir.foreach(dir_web) {|x|
      real_path = File.join(dir_web, x)
      if (!File.directory?(real_path) && File.exists?(real_path))
        if(x == 'WebViewJavascriptBridge.h' || x == 'WebViewJavascriptBridge.m')
          File.delete(real_path)
        end
      end
    }
  end


  


end
