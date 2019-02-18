source 'https://cdn.jsdelivr.net/cocoa/'

platform :ios, '10.0'

use_frameworks!

# ignore all warnings from all pods
inhibit_all_warnings!

install! 'cocoapods', deterministic_uuids: false, generate_multiple_pod_projects: true

target 'DemoPodHeaderSearchPaths' do

  pod 'BraintreeDropIn'

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['EXPANDED_CODE_SIGN_IDENTITY'] = ""
      config.build_settings['CODE_SIGNING_REQUIRED'] = "NO"
      config.build_settings['CODE_SIGNING_ALLOWED'] = "NO"
      config.build_settings['SWIFT_VERSION'] = '4.2'
    end
  end
end
