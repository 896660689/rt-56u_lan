#rt-56u_lan
cd /opt
git clone git@github.com:896660689/padavan-4.4.git

cd /opt/padavan-4.4
git fetch
git checkout -b ad
git branch

cd /opt/padavan-4.4
git checkout main             ## 转到分支
git pull                      ## 拉取远程更新
git branch -D ad3             ## 删除分支
git checkout -b ad8           ## 创建分支
git branch                    ## 查看分支
git push origin ad8:ad8       ## 新分支推送到远程

## 删除无用wap
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_adbyby.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_adguardhome.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_aliddns.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_aliyundrive.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_smartdns.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_zerotier.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/scutclient.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/scutclient_action.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/scutclient_log.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Shadowsocks.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Shadowsocks_action.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Shadowsocks_log.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/scutclient.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/dlink.js
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/disk_functions.js
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Ad_action.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_ddnsto.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/disk_folder_tree.js
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_frp.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_frp_log.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/mentohust.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/mentohust_action.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/mentohust_log.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Ad_action.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_ddnsto.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_frp.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/Advanced_frp_log.asp
rm -rf /opt/padavan-4.4/trunk/user/www/n56u_ribbon_fixed/validator.js

rm -rf /opt/padavan-4.4/trunk/user/shadowsocks/
rm -rf /opt/padavan-4.4/trunk/user/adbyby
rm -rf /opt/padavan-4.4/trunk/user/adguardhome
rm -rf /opt/padavan-4.4/trunk/user/chinadns-ng
rm -rf /opt/padavan-4.4/trunk/user/chnroute
rm -rf /opt/padavan-4.4/trunk/user/dns2tcp
rm -rf /opt/padavan-4.4/trunk/user/dns-forwarder
rm -rf /opt/padavan-4.4/trunk/user/dnsproxy
rm -rf /opt/padavan-4.4/trunk/user/pdnsd
rm -rf /opt/padavan-4.4/trunk/user/redsocks
rm -rf /opt/padavan-4.4/trunk/user/smartdns
rm -rf /opt/padavan-4.4/trunk/user/unblockmusic
rm -rf /opt/padavan-4.4/trunk/user/xray
rm -rf /opt/padavan-4.4/trunk/user/zerotier
git add --all
git commit -m '<del-www.asp>'

cp -r /home/dell/桌面/4.4/.github/ /opt/padavan-4.4/
cp -r /home/dell/桌面/4.4/trunk/ /opt/padavan-4.4/
git add --all                         ## 保存更改
git commit -m '<trunk>'               ## 更改信息
git push --set-upstream origin ad8    ## 本地更新推送到远程

cp -r /home/dell/桌面/4.41/trunk /opt/padavan-4.4/
git add --all
git commit -m '<www>'
git push --set-upstream origin ad8

cp -r /home/dell/桌面/4.44/trunk/ /opt/padavan-4.4/
git add --all
git commit -m '<inadyn>'
git push --set-upstream origin ad8


cp -r /home/dell/桌面/4.42/trunk/ /opt/padavan-4.4/
git add --all
git commit -m '<lbis>'
git push --set-upstream origin ad8

cp -r /home/dell/桌面/4.45/trunk /opt/padavan-4.4/
git add --all
git commit -m '<scripts>'
git push --set-upstream origin ad8


