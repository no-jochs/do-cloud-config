require 'json'
file = './config.json'

desc 'Load configuration from file'
task :configure do
  data = JSON.parse(File.read(file))
  data.each do |key, value|
    ENV[key.to_s] = value.to_s
  end
end
