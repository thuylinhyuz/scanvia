pkg update
pkg install proot-distro -y
proot-distro install ubuntu
proot-distro login ubuntu
termux-setup-storage
apt update
apt upgrade -y
apt install software-properties-common wget curl -y
add-apt-repository ppa:deadsnakes/ppa -y
apt update
apt install python3.12 python3.12-venv python3.12-dev python3-pip -y
python3.12 -V
cd /sdcard/Download
python3.12 -m ensurepip
python3.12 -m pip install requests mechanize rich bs4 html5lib httpx

