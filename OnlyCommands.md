**How to check your current location**
pwd

---

**How to display files and directory present in current location**
ls
ls ~
ls /home/mohd-kaif/
ls ..
ls ../..
ls -l
ls -lt 
ls -ltr
ls -a
ls -al
ls -lS
ls Documents/*.html
ls Documents/*.*
ls -lS > out.txt
ls -d */
ls -R
ls -l -h
ls -lh
ls -ld Desktop/

---

**How to change path or move to another folder in linux**
cd
cd /
cd /home/mohd-kaif/
cd ..
cd ../..
cd ~
cd My\ books
cd "My books"
cd 'My books'

---

**How to copy and paste a file from one folder to another folder in linux**
cp file1.txt file2.txt dir1
cp -i file1.txt file2.txt dir1
cp source destination-path
cp file1.txt dir1

---

**How to copy content of a file to another file in linux**
cp file1.txt file2.txt

---

**How to display content of a file on terminal**
cat text.txt (read)
cat text.txt text.txt
cat -b text.txt
cat -n text.txt (show lines number wise)
cat -s text.txt
cat -E text.txt
cat > text.txt (write)
cat text1.txt text2.txt > out.txt
cat >> text.txt (append)
cat /etc/group

---

**How to create directory or folder in linux**
mkdir image/mark
mkdir -p names/mark
mkdir -p names/{kaif, mohd, mohdkaif}
mkdir -p a/b/c/d
mkdir -v <foldername>
mkdir -m a=r test

---

**How to delete a directory or folder in linux**
rmdir -p a/b/c/d
rmdir -pv a/b/c/d
rmdir <foldername>

---

**How to delete a file in linux**
rm -r <foldername>
rm -rv <foldername>
rm -rf <foldername>
rm -i file
rm -iv file
rm -r folder
rm -rf file
rm -d folder
rm text.txt

---

**How to clear the linux terminal**
clear
ctrl+l

---

**How to cut-paste a file from one folder to another in linux**
mv file.txt destination-path

---

**How to rename a file in linux**
mv fileA.txt fileB.txt

---

**How to display name of current logged-in user**
whoami

---

**How to create a file in linux**
touch file.txt

---

**How to check system date or time**
date
date +%D
date +%T
date +%H:%M

---

**How to read a file and search for a word**
less file.txt 
(then type **/searchWord or ?searchWord** you want to search for and press **n** for next line where word occur and also you can use (shift+g) to goto end of file and press p to goto beginning of file, / is used to search from top to bottom and ? is used to search from bottom to top and press q for exit file)

---

**How to view content of file page by page**
more file.txt (then press down arrow key to view content page by page)

---

**How to edit a file in linux**
vim file.txt
nano file.txt
(ctrl + D for end of file (exit in vim))

---

**How to read or display top 5 lines from a file in linux**
head -5 file.txt

---

**How to read or display bottom 5 lines from a file in linux**
tail -5 file.txt

---

**How to SORT the content from a file in linux**
sort file
sort -r file

---

**How to display UNIQUE content from a file in linux**
sort file.txt | uniq

---

**A file has 9 lines. How to split this file in 3 different files in linux**
split -l 3 file.txt

---

**How to search a word and display matching content from a file in linux**
grep "word" file.txt

---

**How to search multiple words and display matching content from a file in linux**
egrep "word1|word2" file.txt

---

**How to use WILDCARDS in linux * [] {}**
ls *.txt
ls x*
touch file{1..5}

---

**How to SHUFFLE content of file in linux**
shuf file.txt

---

**How to COUNT no. of lines in a file in linux**
wc -l file.txt

---

**How to check if two files are identical or not in linux**
cmp fileA.txt fileB.txt

---

**How to compare and display difference between two files in linux**
diff -u fileA.txt fileB.txt

---

**How to find a file in linux**
find /path/ -name file.txt


---

**How to find a file in linux using locate**
updatedb
locate file.txt

---

**How to display previously used commands in past**
history

---

**How to check syntax and options availbale for a command**
ls --help

---

**How to read or get more info about a command**
man ls

---

**How to check which executable is using for a command**
which ls

---

**How to use calculator in linux**
bc

---

**How to check CALENDER of last year in linux**
cal
cal year
cal month year

---

**How to check How Long server has been running in linux**
uptime

---

**How to record your activity on terminal in a file**
script
(ctrl + d) script done

---

**How to create a short-cut of a long command in linux**
alias l="ls -ltr"
alias -p

---

**How to compress a file in linux**
gzip -k file.txt
zip file.zip file1.txt file2.txt 
zip -r file.zip file1.txt file2. test/
zip -e password.zip file1.txt
zip -m file.zip file1.txt file2.
---

**How to decompress a file in linux**
gzip -d file.txt
gunzip file.txt
unzip file.zip file1.txt
unzip file.zip -d /home/mint/zip_files
unzip -q file.zip 
unzip -l file.zip

---

**How to compress a folder in linux**
tar -czf file.tar.gz dir/

---

**How to decompress a folder in linux**
tar -xzf file.tar.gz

---

**How to compress multiple files in one zipped file in linux**
zip files.zip file1.txt file2.txt

---

**How to decompress multiple files from a one zipped file in linux**
unzip files.zip

---

**How to list files in zipped file**
unzip -l myfiles.zip

---

**How to download a file from internet**
wget URL_of_file
wget -O opt_file.txt URL_of_file

---

**How to call an API on linux**
curl URL

---

**How to install an application on linux**
sudo apt or yum/dnf install application_name

---

**How to check if an application is installed or not on linux**
rpm -qa | grep package_name
dnf list installed | grep package_name

---

**How to list available packages to install on linux**
apt serach package_name
yum/dnf list available | grep package_name

---

**How to start/stop a service on linux**
systemctl start/stop service_name

---

**How to list all services on linux**
systemctl list-units --type=service --all

---

**How to list all existing Environment Variables on linux**
printenv

---

**How to ADD a new Environment Variables on linux**
export VAR_NAME="/usr/lib/jvm/java_v"
export PATH=$VAR_NAME/bin:$PATH

---

**How to ADD a new Environment Variables permanently on linux**
Add env variable in ./bashrc file
source ~/.bashrc_profile

---

**How to print a specific column from a csv file**
awk -F , '{print $2}' file.csv

---

**How to display starting two characters of all line**
cut -c1-2 file.txt

---

**How to display a specific line from a file**
sed -n '5p' file.txt

---

**How  to replace a specific word within a file**
sed -n 's/from/to/g' file.txt

---

**How to convert the content to uppercase or lowercase within a file**
tr [:lower:] [:upper:] < file.txt
tr [:punct:] z < file.txt
tr [:digit:] z < file.txt
tr -d % < file.txt
tr -d "%" "&" < file.txt

---

**How to extend or shrink size of a file**
truncate -s 100M file.txt

---

**How to display following line in vertical line?ABCDE**
echo "ABCDE" | fold -w1

---

**How to change user or login as different user in linux**
su user_name
su user_name
passwd username
groupadd <group_name>
sudo groupadd -f -g 2022 dev

---

**How to exit as current user or close terminal in linux**
exit

---

**If you are not root user, how to execute adimin commands like installing new apps**
sudo yum install app_name

---

**How to access remote linux server**
ifconfig
ssh user_name@ip_address

---

**How to copy a file to a remote linux server**
scp file.txt user_name@ip_address:/tmp/

---

**How to check permissions of a file**
ls -ltr

---

**How to modify permissions of a file**
chmod a+rwx file.txt
(u - user, g - group, o - others, a - all)
chmod +r <filename>/<foldername>
chmod +w <filename>/<foldername>
chmod +x <filename>/<foldername>
chmod -r <filename>/<foldername>
oldername
chmod -w <filename>/<foldername>
chmod -x <filename>/<foldername>
chmod 777 <filename>/<foldername>
chmod +xwr <filename>/<foldername>
chmod u=r/g=r/o=r <filename>/<foldername>
chmod u+r/g+r/o+r <filename>/

---

**How to change ownership of a file**
chown user_name file.txt

**How to change group ownership of a file**
chgrp group_name file.txt

---

**How to check free RAM space**
free
free -h
free -m

---

**How to check %memory and CPU utilization**
top

---

**How to check disk utilization**
du
du -h
du -h foler/

---

**How to check filesystem available and disk space allocated**
df
df -h

---

**How to check hostname of your linux server**
hostname

---

**How to check cpu/core/thread info of your linux server**
lscpu

---

**How to check type of architecture of your linux server**
arch

---

**How to see list of storage devices, disk partition on your linux server**
lsblk

---

**How to see OS name of linux server**
uname -a
cat /etc/os-release

---

**How to check if a precess(java) is running or not**
ps -ef | grep process_name

---

**How to get PID of a process**
pgrep process_name

---

**How to stop a process by PID**
kill -9 PID

---

**How to stop a process by its name**
pkill process_name

---

**How to see all the active jobs**
jobs

---

**How to resume a job in background**
bg

---

**How to resume a job in foreground**
fg

---

**How to run a scrip in background**
nohup ./script >dev/null &

---

**How to check IP of you machine**
ifconfig

---

**How to check if a server or website is accesible or not**
ping www.google.com

---

**How to check if a IP:PORT is accessible and open or not**
telnet IP PORT

---

**How to check if port is open or not on our server**
netstat -putan | grep PORT

---

**How to check all hubs in network path to reach a website**
traceroute www.google.com

---

**How to restart our linux server**
reboot

---

**How to shutdown our linux server**
shutdown

---

**How to create a new user on our linux server**
useradd user_name

---

**How to change password for the user**
passwd user_name

---

**How to create a new group on our linux server**
groupadd group_name

---

**How to check UserId or GroupID of a user**
id user_name

---

**How to delete user or group**
userdel user_name
groupdel group_name
userdel -r (will remove home directory)
userdel -f (force delete even if the user is logged in)
(To add user to a new group, but default group will remain same)
usermod -G <group_name> <user_name>
**_To change the default group_**
usermod -g <group_name> <user_name>
less /etc/group
(
  other flags for usermod
  1. -p (we use passwd command also)
  2. -s (shell type)
  3. -l -U (lock/ Unlock a user)
  4. -m -d /home/newfolder (to move the content of home folder to this new folder)
)
less /etc/passwd
less /etc/shadowgroup

---

**How to change the group of user**
usermod -g group_name user_name

---

**How to schedule a script to run on a particular date/time**
at 10:00 PM
crontab -e

---

**How to move file or folders in recycle bin**
gio trash <foldername>
gio trash text.txt

---

**How to collect all file or folder name in a file**
ls > files_name_location.txt


**id of user or group**
id username
id -g <group_name> -s /bin/bash -c "description" -m -d /home/<user_name> <username>
