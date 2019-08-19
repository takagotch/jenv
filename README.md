### jenv
---
https://github.com/gcuisinier/jenv

```
```

```sh
brew install jenv

echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.bash_profile
echo 'eval "$(jenv init -)"' >> ~/.bash_profile
echo 'export PATH="$HOME/.jenv/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(jenv init -)"' >> ~/.zshrc

jenv doctor
jenv enable-plugin export
exec $SHELL -l
echo 'set PATH $HOME/.jenv/bin $PATH' >> ~/.conf/fish/config.sh
cp ~/.jenv/fish/jenv.fish ~/.conf/fish/function/export.fish
brew cask install java
jenv add $(/usr/libexec/java_home)

jenv versions
jenv local 11.0.2
exec $SHELL -l
cat .java-version
echo ${JAVA_HOME}

rm .java-version
jenv global 11.0.2
jenv shell 11.0.2
brew tap caskroom/versions
brew cask install java8
ls -l /Library/Java/JavaVirtualMachines
jenv add /Library/Jva/JavaVirtualMachines/jdk1.8.0._202.jdk/Contents/Home/
jenv versions
jenv shell 1.8
java -version
```

```
```


