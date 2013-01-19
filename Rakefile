desc "Setup vimrc files as janus needs"
task :install do

  links = %w(vimrc.before gvimrc.before vimrc.after gvimrc.after )

  links.each do |link|
    link_path = "~/.#{link}"
    target_path = "~/.janus/#{link}"
    
    sh "rm #{link_path}" if File.exists? link_path
    sh "ln -s #{target_path} #{link_path}"
  end

end

desc "Install distribution"
task :install_janus do
  sh "curl -Lo- https://bit.ly/janus-bootstrap | bash"
end


