desc "Rakefile task for testing"
task default: ["test"]

require 'html-proofer'
desc 'test links in the build web site'
task :test do
  sh "bundle exec jekyll build"
  options = {
    :assume_extension => true,
    :external_only => true,
  }
  HTMLProofer.check_directory("./_site", options).run
end