![スクリーンショット 2019-07-12 8 59 47](https://user-images.githubusercontent.com/5633085/61093278-b3c23b80-a484-11e9-974f-ca173732bc5d.png)

# How to

## 1.fork run first.sh  
````
Fork!!!!
$ ./scripts/first.sh
````

## 2.dry-run
````
$ ansible-playbook -i hosts mac.yml -KD -C
````

## 3.run
````
$ ansible-playbook -i hosts mac.yml -KD
````
## 4.reboot Mac

😎

## tag run

If you want to run each role after the second time, you can also run with tags.

- homebrew
```
$ ansible-playbook -i hosts mac.yml --tags homebrew -KD

```
- homebrew-cask
```
$ ansible-playbook -i hosts mac.yml --tags homebrew-cask -KD

```
- homedirectory
```
$ ansible-playbook -i hosts mac.yml --tags homedirectory -KD

```
