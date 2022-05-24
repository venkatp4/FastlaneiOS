# Uncomment the next line to define a global platform for your project
 platform :ios, '13.0'
 source 'https://github.com/CocoaPods/Specs.git'
 
  target 'FastLaneExample' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for FastLaneExample
  pod 'Firebase'
  
  target 'FastLaneExampleTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'FastLaneExampleUITests' do
    # Pods for testing
  end
end

post_install do |installer_representation|
    installer_representation.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['ALWAYS_EMBED_SWIFT_STANDARD_LIBRARIES'] = '$(inherited)'
        end
    end
end
