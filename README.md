# JavaPath
Здесь описаны варианты добавления пути до Java в различных ОС


1) **Linux**  
* если необходимо указать путь до Java просто в рамках данной сессии/подключения на Linux, то в консоли прописать следующие строки:  
<sub> export JAVA_HOME=/opt/jdk-11</sub>  
<sub> export PATH=$JAVA_HOME/bin:$PATH</sub> 
* если необходимо указать путь до Java на постоянку, то в .profile или в .bashrc (лежат в домашнем каталоге ~) добавить следующие строки:  
<sub> export JAVA_HOME=/opt/jdk-11</sub>  
<sub> export PATH=$JAVA_HOME/bin:$PATH</sub>  
-> затем выполнить команду:  
<sub> source .profile или же source .bashrc</sub>  
* а для автоматизации через баш скрипт необходимо в него добавить следующие строки:  
<sub> sudo sh -c "echo 'export JAVA_HOME=\"/u01/jdk11\" export PATH=\$JAVA_HOME/bin:\$PATH' >> ~/.profile"</sub>    
  
2) **Windows**  
* если необходимо указать путь до Java просто в рамках данной сессии/подключения на Windows (н-р в окне IntellijIdea), то в окне прописать следующие строки:  
<sub> SET JAVA_HOME=C:\Program Files\Java\jdk-11.0.8</sub>  
<sub> SET PATH=%JAVA_HOME%\bin;%PATH%</sub>  
