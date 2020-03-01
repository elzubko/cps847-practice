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
\ntravis encrypt-file deploy_rsa --add
\nchmod 644 deploy_rsa.pub
\ncat deploy_rsa.pub >> ~/.ssh/authorized_keys
\nrm deploy_rsa deploy_rsa.pub
\ngit add deploy_rsa.enc
\ngit commit -m "yuh"
