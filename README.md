# app-engine-start-vm
Use App Engine to start a Compute Engine VM

## Instruction
登录cloud shell:

mkdir start-stop-gcp //建立一个文件夹

cd start-stop-gcp

git clone https://github.com/xmlf/app-engine-start-vm.git

cd app-engine-start-vm/

pip install -t lib oauth2client

pip install --upgrade google-api-python-client

pip install -t lib oauth2client

pip install --upgrade google-api-python-client -t lib

//pip install -r requirements.txt -t lib

nano cron.yaml
//复制启动代码，分别修改开机和关机时间

nano main.py
//修改实例名称、地区和VM实例项目ID，并复制开机代码一份，修改为关机代码。

gcloud app deploy app.yaml cron.yaml --project [项目id]

