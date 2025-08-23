# A sample Guardfile is more complex and can define different tasks to be run
# when files are modified. Here are some examples:

# Guard::Minitest
guard :minitest do
  # Rails
  watch(%r{^app/(.+)\.rb$})                               { |m| "test/#{m[1]}_test.rb" }
  watch(%r{^app/controllers/application_controller\.rb$})  { 'test/controllers' }
  watch(%r{^app/controllers/(.+)_controller\.rb$})         { |m| "test/integration/#{m[1]}_test.rb" }
  watch(%r{^app/views/(.+)_mailer/.+})                    { |m| "test/mailers/#{m[1]}_mailer_test.rb" }
  watch(%r{^app/helpers/(.+)_helper\.rb$})                { |m| "test/helpers/#{m[1]}_helper_test.rb" }
  watch(%r{^lib/(.+)\.rb$})                               { |m| "test/lib/#{m[1]}_test.rb" }
  watch(%r{^test/.+_test\.rb$})
  watch(%r{^test/test_helper\.rb$})                       { 'test' }

  # Capybara integration tests
  watch(%r{^app/views/(.+)/.*\.erb$})                     { |m| "test/integration/#{m[1]}_test.rb" }
  watch(%r{^app/helpers/(.+)_helper\.rb$})                { |m| "test/integration/#{m[1]}_test.rb" }
end

# Guard::RSpec
# guard :rspec do
#   watch(%r{^spec/.+_spec\.rb$})
#   watch(%r{^lib/(.+)\.rb$})     { |m| "spec/lib/#{m[1]}_spec.rb" }
#   watch(%r{^spec/.+_spec\.rb$}) { |m| "spec/#{m[1]}_spec.rb" }
# end

# Guard::Jasmine
# guard :jasmine do
#   watch(%r{spec/javascripts/.*_spec\.(coffee|js)$})
#   watch(%r{app/assets/javascripts/(.+)\.(coffee|js)$}) { |m| "spec/javascripts/#{m[1]}_spec.#{m[2]}" }
# end

# Guard::Livereload
# guard :livereload do
#   watch(%r{app/views/.+\.erb$})
#   watch(%r{app/assets/stylesheets/(.+)\.css$})
#   watch(%r{app/assets/javascripts/(.+)\.js$})
# end
