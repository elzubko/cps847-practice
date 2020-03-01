# cps847-practice
Midterm Practice
## Moon Deployment
mkdir cps847
cd cps847
git clone https://github.com/username/repo.git
cd repo
ssh-keygen -t rsa -b 4096 -C 'build@travis-ci.org' -f ./deploy_rsa
##### enter
##### enter
##### travis encrypt-file deploy_rsa --add
##### chmod 644 deploy_rsa.pub
##### cat deploy_rsa.pub >> ~/.ssh/authorized_keys
##### rm deploy_rsa deploy_rsa.pub
##### git add deploy_rsa.enc
##### git commit -m "yuh"
