require 'rubygems'
require 'rake'

begin
  require 'jeweler'
  Jeweler::Tasks.new do |gem|
    gem.name = "rb-pygments"
    gem.summary = %Q{A Ruby wrapper for the Pygments syntax highlighter.}
    gem.description = gem.summary
    gem.email = "nex342@gmail.com"
    gem.homepage = "http://github.com/nex3/rb-pygments"
    gem.authors = ["Nathan Weizenbaum"]
    gem.add_development_dependency('yard', '~> 0.5.3')
    gem.requirements << 'pygments, 1.2.2 or greater'
    # gem is a Gem::Specification... see http://www.rubygems.org/read/chapter/20 for additional settings
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler (or a dependency) not available. Install it with: gem install jeweler"
end

begin
  require 'yard'
  YARD::Rake::YardocTask.new
rescue LoadError
  task :yardoc do
    abort "YARD is not available. In order to run yardoc, you must: sudo gem install yard"
  end
end
