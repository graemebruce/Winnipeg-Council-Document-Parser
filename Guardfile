guard :rspec, cmd: 'bundle exec rspec' do
  watch(%r{^spec/.+_spec\.rb$})
  watch('spec/spec_helper.rb')  { 'spec' }
  watch(%r{^(.+)\.rb}) { |m| "spec/#{m[1]}_spec.rb" }
end

guard :rubocop, cli: ['-c', 'rubocop.yml'] do
  watch(%r{.+(\.rb)$})
end
