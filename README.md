pip
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py --user

pip install docker

docker volume create es_storage

docker network create network001
docker network create network002
docker network create network003

ansible-playbook beats.yml --tags es
