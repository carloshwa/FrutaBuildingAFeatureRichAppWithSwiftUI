platform :ios, '15.0'
use_frameworks!

target 'Fruta iOS' do
end

target 'Fruta iOS Clip' do
end

target 'Fruta iOS Widgets' do
end

post_install do |installer|
    installer.pods_project.targets.each do |target|
      target.build_configurations.each do |config|
        config.build_settings['EXCLUDED_ARCHS[sdk=iphonesimulator*]'] = 'arm64'
      end
    end
end
