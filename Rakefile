desc "Setup vimrc files as janus needs"
task :install do

  sh "rm ~/.vimrc.before"
  sh "rm ~/.vimrc.after"

  sh "rm ~/.gvimrc.before"
  sh "rm ~/.gvimrc.after"

  sh "ln -s ~/.janus/vimrc.before ~/.vimrc.before"
  sh "ln -s ~/.janus/gvimrc.before ~/.gvimrc.before"

  sh "ln -s ~/.janus/vimrc.after ~/.vimrc.after"
  sh "ln -s ~/.janus/gvimrc.after ~/.gvimrc.after"

end
