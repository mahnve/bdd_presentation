task :default => :build

task :build do
  `svgslides -i list`
end

task :view => :build do
  `evince slides.pdf`
end

task :present => :build do
  IO.popen "impressive -t Crossfade slides.pdf"
end
