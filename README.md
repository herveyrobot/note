# note  
github learning note  

#about connect the github  
##First step: ssh key  
 ssh-keygen -t rsa -C "email adress"  
then  
 enter password(twice)  
(the id_rsa is private ,and the id_rsa.pub is public)  

##Second step: name and address  
git config --globle user.name "username"  
git config --globle user.email "email address"  

we can check by "~./gitconfig"  

##for the good feeling about reading  
git config --globle color.ui auto  

check by "~./gitconfig"  
##examine password  
cat ~./ssh/id_rsa.pub

##connection  
ssh -T git@github.com

##clone  
git clone git@github.com:username/repository_name.com  
cd repository_name  

##submit  
eg:hello_world.php  
###coding  
<?php  
     echo "Hello World"  
?>  
  
git status  
git add hello_world.php  
git commit -m "Add hello world script by php"  

###check log  
git log  

git push  

##modidy README.md  
 git add README.md  
 git commit -m "modify README.md"  
 git log  
 git push  
