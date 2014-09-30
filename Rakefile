require 'rubygems'
require 'rake'
require 'rdoc'
require 'date'
require 'yaml'
require 'tmpdir'
require 'jekyll'


desc "Starting Web Server"
task :server do 
    puts "Starting Web Server http://127.0.0.1:3000"
	system "jekyll serve --watch"
end

desc "Generating website from source"
task :compile do 
    puts "Generating website. output: _deploy"
    system "jekyll build"
end

desc "Generating static files and watching output: _deploy"
task :build do
   puts "Generating static files and watching output: _deploy"
   system "jekyll build --watch"
end


# For FTP user
desc "Deploy website"
task :deploy do
    puts "Deploying website"
    system "glynn"
end


## For GitHub pages user.

    desc "Generate and publish blog to gh-pages"
    task :publish => [:generate] do
      Dir.mktmpdir do |tmp|
        system "mv _deploy/* #{tmp}"
        system "git checkout -B gh-pages"
        system "rm -rf *"
        system "mv #{tmp}/* ."
        message = "Site updated at #{Time.now.utc}"
        system "git add ."
        system "git commit -am #{message.shellescape}"
        system "git push origin gh-pages --force"
        system "git checkout master"
        system "echo yolo"
      end
    end

task :default => :publish
