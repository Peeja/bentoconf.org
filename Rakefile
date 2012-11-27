desc "Generate site."
task :generate do
  sh "jekyll"
end

desc "Deploy live site."
task :deploy => :generate do
  sh "rsync -avz --delete site/ peeja_bentoconf@ssh.phx.nearlyfreespeech.net:/home/public"
end
