use_frameworks!

workspace 'R.swift'
project 'ResourceApp/ResourceApp'

target 'ResourceApp'
target 'ResourceAppTests'

pod 'R.swift.Library', :git => 'https://github.com/bre7/R.swift.Library.git'

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '3.0'
    end
  end
end
