# A sample Guardfile
# More info at https://github.com/guard/guard#readme

guard 'coffeescript', :input => 'source/javascripts', :output => 'html/javascripts'

guard 'less', :all_on_start => true, :all_after_change => true, :output => 'html/stylesheets'  do
  watch(%r{^.+\.less$})
end

guard 'sass', :input => 'source/stylesheets', :output => 'html/stylesheets'

guard 'haml', :input => 'source', :output => 'html' do
  watch(/^.+(\.html\.haml)/)
end
