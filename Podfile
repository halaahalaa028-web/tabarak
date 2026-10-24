# Uncomment the next line to define a global platform for your project
platform :ios, '15.0'

# Firebase Messaging's Swift dependencies need module maps when linked statically.
use_modular_headers!

target 'تبارك فارما' do
  # Keep CocoaPods on its default static-library integration to avoid the
  # malformed aggregate framework linker flag produced for the Arabic target.
  pod 'Firebase/Messaging'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '15.0'
    end
  end
end
