#请修改Dockerfile中的env环境变量，分别对应用户的config文件以及ansible-playbook文件夹路径。
#Please edit the ENV in Dockerfile with the paths of your .ssh/config and ansible-playbook.
#使用方法:
1.	docker build -t kevin/ansible .
2.	docker run -it -v ~/.ssh:/home/kevin/.ssh -v ~/server-config:/home/kevin/server-config --name ansible kevin/ansible /bin/bash
