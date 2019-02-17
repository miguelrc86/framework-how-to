platform :ios, '12.1'

target 'KnobShowcase' do
  use_frameworks!

  pod 'KnobControl', :git => 'https://github.com/miguelrc86/leKnobControl', :tag => '1.0.0'

end

# Workaround for Cocoapods issue #7606
post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        config.build_settings.delete('CODE_SIGNING_ALLOWED')
        config.build_settings.delete('CODE_SIGNING_REQUIRED')
    end
end
