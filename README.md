# Installing maven

cd /opt

wget https://downloads.apache.org/maven/maven-3/3.6.3/binaries/apache-maven-3.6.3-bin.tar.gz

tar -xvzf apache-maven-3.6.3-bin.tar.gz

mv apache-maven-3.6.3 maven


# Installing JAVA

sudo apt update

sudo apt install openjdk-8-jdk


# Exporting the path

vi ~/.bashrc

# Add the following configuration 

#bash_profile

#get the aliases and functions

if [ -f ~/.bashrc ]; then
. ~/.bashrc
        
fi

#user specific environment and startup programs

export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-amd64\

export M2_HOME=/opt/maven

export M2=/opt/maven/bin

export PATH=$PATH:$HOME/bin/:$JAVA_HOME:$M2:$M2_HOME

export PATH



# Save the bashrc 

:wq!

source  ~/.bashrc

# Now go to Jenkins and download the following plugins

1. Maven integration 

2. Maven invoker







