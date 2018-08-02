Bundler.require :default

guard 'shell' do
  # watch(/^mydoc\.adoc$/) {|m|
  watch(/^.*\.adoc$/) {|m|
    Asciidoctor.convert_file m[0]
  }
end

guard 'livereload' do
  watch(%r{^.+\.(css|js|html)$})
end
