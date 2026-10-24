# Uncomment the next line to define a global platform for your project
platform :ios, '15.0'

target 'تبارك فارما' do
  # Use CocoaPods' default static-library integration.
  # Avoid use_frameworks! because the Arabic target name creates an invalid
  # aggregate framework linker flag (Pods____________) during the iOS archive.
  pod 'Firebase/Messaging'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '15.0'
    end
  end
end
