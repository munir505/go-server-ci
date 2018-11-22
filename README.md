# go-server-ci
Automated CI setup using Docker
(Continuous Integration)

To Install Docker Compose:
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Then, make it an executable:
```bash
sudo chmod +x /usr/local/bin/docker-compose
```
The Pipeline can be created using docker-compose:
```bash
docker-compose up -d
```
Jenkins will accessible from port 80

When a branch has been built with the included Jenkins job
It can be accessed from `/go-server/branch-name`
For example to connect to the deployed master branch:
`/go-server/master`

To change and make branches, clone the 'go-server' repo:
```bash
git clone https://github.com/munir505/go-server
```
Then make a branch:
```bash
git checkout -b <branch_name>
```
Then make changes to the files, after push the changes to that branch:
```bash
git push -u origin <branch_name>
```
