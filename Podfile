# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'parseInstaClone' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

pod 'Parse'
pod 'FSCalendar'
pod 'Eureka'

  # Pods for parseInstaClone

post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['APPLICATION_EXTENSION_API_ONLY'] = 'No' 
      end
   end

 installer.generated_projects.each do |project|
          project.targets.each do |target|
              target.build_configurations.each do |config|
                  config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
               end
          end
   end
end

end
