require 'rake/gempackagetask'

spec = Gem::Specification.new do |s| 
  s.name = "moneta-namespace"
  s.version = "0.0.3"
  s.author = "Roger Jungemann"
  s.email = "roger@thefifthcircuit.com"
  s.homepage = "http://github.com/thefifthcircuit/moneta-namespace"
  s.platform = Gem::Platform::RUBY
  s.summary = "Define multiple namespaces when using Moneta."
  s.description = s.summary
  s.files = FileList["{bin,lib,vendor}/**/*"].to_a
  s.require_path = "lib"
  #s.autorequire = "name"
  #s.test_files = FileList["turnstile_spec.rb"].to_a
  s.has_rdoc = false
  #s.extra_rdoc_files = ["LICENSE.txt, README.txt"]
  s.add_dependency("moneta")
end
 
Rake::GemPackageTask.new(spec) do |pkg| 
  pkg.need_tar = true 
end