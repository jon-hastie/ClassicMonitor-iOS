# Uncomment the next line to define a global platform for your project
 platform :ios, '14.0'

target 'Classic' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  #pod 'LMGaugeViewSwift'
  # Pods for Classic

  #To Get Classics Over the Network
  pod 'CocoaAsyncSocket'

  #MQTT
  pod 'MQTTClient/Min'
  pod 'MQTTClient/Manager'
  pod 'MQTTClient/Websocket'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '14.0'
      config.build_settings['CLANG_WARN_QUOTED_INCLUDE_IN_FRAMEWORK_HEADER'] = 'NO'
    end
  end
  installer.pods_project.build_configurations.each do |config|
    config.build_settings['GCC_WARN_INHIBIT_ALL_WARNINGS'] = 'YES'
    config.build_settings['CLANG_WARN_QUOTED_INCLUDE_IN_FRAMEWORK_HEADER'] = 'NO'
  end
end
