namespace :build do
  desc 'Generate HTML outputs'
  task :html do
    puts "Converting to HTML..."
    `bundle exec asciidoctor src/oficina_git.adoc -o oficina_git.html`
    puts " -- HTML output at oficina_git.html"
  end

  desc 'Generate PDF outputs'
  task :pdf do
    puts "Converting to PDF... (this one takes a while)"
    `bundle exec asciidoctor-pdf src/oficina_git.adoc -o oficina_git.pdf`
    puts " -- PDF  output at oficina_git.pdf"
  end
end

desc 'Build all default formats'
task :build => [ "build:html", "build:pdf" ]
