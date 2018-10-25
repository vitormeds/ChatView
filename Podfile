project 'ChatView.xcodeproj'

# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'ChatView' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  pod 'MessageKit'
  pod 'Firebase/Core'
  pod 'Firebase/Messaging'
  pod 'Firebase/Database'
  pod 'SwiftyJSON'
  use_frameworks!

  # Pods for ChatView

  target 'ChatViewTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'ChatViewUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
    installer.pods_project.targets.each do |target|
        if target.name == 'MessageKit'
            target.build_configurations.each do |config|
                config.build_settings['SWIFT_VERSION'] = '4.0'
            end
        end
    end
end
