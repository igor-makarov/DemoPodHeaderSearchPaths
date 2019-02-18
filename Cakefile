require 'yaml'

project.name = 'DemoPodHeaderSearchPaths'

application_for :ios, '10.0' do |target|
  target.name = 'DemoPodHeaderSearchPaths'
  target.all_configurations.each do |config|
    config.product_bundle_identifier = 'com.igor.demopodheadersearchpaths'
  end
end

project.after_save do
  system "rm -rf \"#{project.name}.xcodeproj/xcshareddata/xcschemes\""
end
