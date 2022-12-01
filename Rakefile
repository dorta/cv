# Copyright 2019-2022 Diego Dorta

namespace :build do
task :pdf do
`bundle exec asciidoctor-pdf -apdf-style=themes/custom-theme.yml -a pdf-fontsdir=themes/fonts DiegoDortaCV.adoc -o docs/DiegoDortaCV.pdf`
end
task :html do
`bundle exec asciidoctor DiegoDortaCV.adoc -o docs/DiegoDortaCV.html`
end
end
desc 'Build all default formats'
task :build => [ 'build:html', 'build:pdf' ]
