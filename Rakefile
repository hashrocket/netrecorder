require 'rubygems'
require 'rake'
require 'echoe'

Echoe.new('hashrocket-netrecorder', '0.2.1') do |p|
  p.description    = "Record network responses for easy stubbing of external calls"
  p.url            = "http://github.com/hashrocket/netrecorder"
  p.author         = "Chris Young, Josh Graham, Jim Remsik"
  p.email          = "dev@hashrocket.com"
  p.ignore_pattern = ["tmp/*", "script/*"]
  p.development_dependencies = %w(echoe cucumber rspec)
  p.runtime_dependencies = %w(fakeweb)
end

Dir["#{File.dirname(__FILE__)}/tasks/*.rake"].sort.each { |ext| load ext }
