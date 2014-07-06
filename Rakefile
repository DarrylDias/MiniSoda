require "rubygems"

desc "Starting Web Server"
task :server do 
    puts "Starting Web Server http://127.0.0.1:3000"
	system "jekyll serve --watch"
end

desc "Generating static files"
task :build do
   puts "Generating website in _deploy"
   system "jekyll build"
end

desc "Deploy website"
task :deploy do
    puts "Deploying website"
    system "glynn"
end