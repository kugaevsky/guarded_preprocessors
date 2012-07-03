# A sample Guardfile
# More info at https://github.com/guard/guard#readme

# -= Guard notifications =-

# notification :growl
# notification :libnotify, :timeout => 5, :transient => true, :append => false, :urgency => :critical
# notification :notifu, :time => 5, :nosound => true, :xp => true

# -= Guard preprocessors =-

group :templates do
  guard 'haml', :input => 'source', :output => 'html' do
    watch(/^.+(\.html\.haml)/)
  end
end

group :javascripts do
  guard 'coffeescript', :input => 'source/javascripts', :output => 'html/javascripts'
end

group :stylesheets do
  guard 'less', :all_on_start => true, :all_after_change => true, :output => 'html/stylesheets'  do
    watch(%r{^.+\.less$})
  end

  guard 'sass', :input => 'source/stylesheets', :output => 'html/stylesheets'
end
