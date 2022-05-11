# ansible-isucon/isucon5-qualifier

## Overview

Ansible playbook for [ISUCON5-qualifier](http://isucon.net/archives/45166636.html)

## Requirement

- Ubuntu 16.04

## Usage

Remote:
```
git clone https://github.com/matsuu/ansible-isucon.git
cd ansible-isucon/isucon5-qualifier
${EDITOR} remote
ansible-playbook -i remote playbook.yml
```

Local:
```
apt-add-repository ppa:ansible/ansible
apt update
apt install git ansible
git clone https://github.com/matsuu/ansible-isucon.git
cd ansible-isucon/isucon5-qualifier
# for image
ansible-playbook -i local image/ansible/playbook.yml
# for bench
ansible-playbook -i local bench/ansible/playbook.yml
```

## 本来の設定と異なるところ

- ベンチマークはCLIから手動で実行する必要があります
- goのバージョンを依存関係解決のため1.5から1.8に変更しています

## References

- [ISUCON5 予選レギュレーション](http://isucon.net/archives/45347574.html)
- [ISUCON5 予選マニュアル](https://gist.github.com/tagomoris/1a2df5ab0999f5e64cff)
- [isucon/isucon5-qualify](https://github.com/isucon/isucon5-qualify)
- [vagrant-isucon](https://github.com/matsuu/vagrant-isucon)
