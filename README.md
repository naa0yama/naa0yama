# Hi there 👋

## Blog posts
<!-- BLOG-POST-LIST:START -->
[MikroTik upgrade 7.4.0 to 7.5.0](https://blog.aoya6i.com/mikrotik-upgrade-740-to-750): 2022-09-13 &lt;p&gt;&lt;/p&gt;
&lt;ul&gt;
&lt;li&gt;Hardware: CRS310-1G-5S-4S+IN&lt;/li&gt;
&lt;li&gt;Old Version: 7.4.0&lt;/li&gt;
&lt;li&gt;New Version: 7.5.0&lt;/li&gt;
&lt;/ul&gt;
&lt;h1 id=&quot;heading-changelogs&quot;&gt;changelogs &lt;/h1&gt;
&lt;p&gt;&lt;a target=&quot;_blank&quot; href=&quot;https://mikrotik.com/download/changelogs&quot;&gt;MikroTik Routers and Wireless - Software&lt;/a&gt;&lt;/p&gt;
&lt;p&gt;&lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;*&rpar; dns - added &lt;span class=&quot;hljs-string&quot;&gt;&quot;address-list&quot;&lt;/span&gt; parameter &lt;span class=&quot;hljs-keyword&quot;&gt;for&lt;/span&gt; static DNS entries &lpar;CLI only&rpar;;
*&rpar; netwatch - changed ICMP default packet loss fail threshold to 85%;
*&rpar; ssh - fixed importing of public keys;
*&rpar; swos - enabled SwitchOS support &lt;span class=&quot;hljs-keyword&quot;&gt;for&lt;/span&gt; CRS310-1G-5S-4S+;
*&rpar; vrrp - added &lt;span class=&quot;hljs-string&quot;&gt;&quot;sync-connection-tracking&quot;&lt;/span&gt; compatibility with preemption-mode;
*&rpar; vrrp - fixed high CPU usage when &lt;span class=&quot;hljs-string&quot;&gt;&quot;sync-connection-tracking=yes&quot;&lt;/span&gt; and the backup router goes offline;
*&rpar; vrrp - fixed HW offloaded bridge MAC address learning when changing from VRRP master to backup;
*&rpar; vrrp - fixed initial connection tracking synchronization, a backup router now always receives all existing connections;
*&rpar; cloud - &lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt; critical &lt;span class=&quot;hljs-built_in&quot;&gt;log&lt;/span&gt; message when system clock gets synchronized;
*&rpar; console - fixed situation when &lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt; output was not consistent;
*&rpar; ssh - &lt;span class=&quot;hljs-built_in&quot;&gt;disable&lt;/span&gt; ssh-rsa when strong-crypto=yes and use rsa-sha2-sha256;
*&rpar; ssh - fixed host key generation &lpar;introduced &lt;span class=&quot;hljs-keyword&quot;&gt;in&lt;/span&gt; v7.3&rpar;;
*&rpar; ssh - implemented &lt;span class=&quot;hljs-string&quot;&gt;&quot;server-sig-algs&quot;&lt;/span&gt; extension &lt;span class=&quot;hljs-keyword&quot;&gt;in&lt;/span&gt; order to improve rsa-sha2-sha256 support;
&lt;/code&gt;&lt;/pre&gt;
&lt;p&gt;&lt;code&gt;*&rpar; vrrp - fixed HW offloaded bridge MAC address learning when changing from VRRP master to backup;&lt;/code&gt;  bridge  &lt;code&gt;ageing-time=1m&lt;/code&gt;  VRRP &lt;/p&gt;
&lt;p&gt;&lt;/p&gt;
&lt;div class=&quot;embed-wrapper&quot;&gt;&lt;div class=&quot;embed-loading&quot;&gt;&lt;div class=&quot;loadingRow&quot;&gt;&lt;/div&gt;&lt;div class=&quot;loadingRow&quot;&gt;&lt;/div&gt;&lt;/div&gt;&lt;a class=&quot;embed-card&quot; href=&quot;https://blog.aoya6i.com/mikrotik-crs310-1g-5s-4sin-upgrade-723-to-731&quot;&gt;https://blog.aoya6i.com/mikrotik-crs310-1g-5s-4sin-upgrade-723-to-731&lt;/a&gt;&lt;/div&gt;
 

[FS.com s3910-24tf, s3410-10tf-p-01 証明書更新](https://blog.aoya6i.com/fscom-s3910-24tf-s3410-10tf-p-01-certificate-update-from-2022): 2022-07-23 &lt;p&gt;&lt;/p&gt;
&lt;p&gt;&lpar;398 Days &lt;/p&gt;
&lt;h3 id=&quot;heading-https&quot;&gt;https  &lt;/h3&gt;
&lt;p&gt;copy &lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;copy tftp://192.0.2.1/usercert.pem flash:usercert.pem.pem
copy tftp://192.0.2.1/usercert.key flash:usercert.pem.key
&lt;/code&gt;&lt;/pre&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;web-server https certificate pem usercert.crt private-key usercert.key
&lt;/code&gt;&lt;/pre&gt;
&lt;p&gt;&lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;show web-server https certificate information
&lt;/code&gt;&lt;/pre&gt;
 

[MikroTik upgrade 7.3.1 to 7.4.0](https://blog.aoya6i.com/mikrotik-upgrade-731-to-740): 2022-07-23 &lt;p&gt;&lt;/p&gt;
&lt;ul&gt;
&lt;li&gt;Hardware: CRS310-1G-5S-4S+IN&lt;/li&gt;
&lt;li&gt;Old Version: 7.3.1&lt;/li&gt;
&lt;li&gt;New Version: 7.4.0&lt;/li&gt;
&lt;/ul&gt;
&lt;h1 id=&quot;heading-changelogs&quot;&gt;changelogs &lt;/h1&gt;
&lt;p&gt;&lt;a target=&quot;_blank&quot; href=&quot;https://mikrotik.com/download/changelogs&quot;&gt;MikroTik Routers and Wireless - Software&lt;/a&gt;&lt;/p&gt;
&lt;p&gt;&lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;*&rpar; cloud - &lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt; critical &lt;span class=&quot;hljs-built_in&quot;&gt;log&lt;/span&gt; message when system clock gets synchronized;
*&rpar; console - fixed situation when &lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt; output was not consistent;
*&rpar; ssh - &lt;span class=&quot;hljs-built_in&quot;&gt;disable&lt;/span&gt; ssh-rsa when strong-crypto=yes and use rsa-sha2-sha256;
*&rpar; ssh - fixed host key generation &lpar;introduced &lt;span class=&quot;hljs-keyword&quot;&gt;in&lt;/span&gt; v7.3&rpar;;
*&rpar; ssh - implemented &lt;span class=&quot;hljs-string&quot;&gt;&quot;server-sig-algs&quot;&lt;/span&gt; extension &lt;span class=&quot;hljs-keyword&quot;&gt;in&lt;/span&gt; order to improve rsa-sha2-sha256 support;
&lt;/code&gt;&lt;/pre&gt;
&lt;p&gt;&lt;/p&gt;
&lt;div class=&quot;embed-wrapper&quot;&gt;&lt;div class=&quot;embed-loading&quot;&gt;&lt;div class=&quot;loadingRow&quot;&gt;&lt;/div&gt;&lt;div class=&quot;loadingRow&quot;&gt;&lt;/div&gt;&lt;/div&gt;&lt;a class=&quot;embed-card&quot; href=&quot;https://blog.aoya6i.com/mikrotik-crs310-1g-5s-4sin-upgrade-723-to-731&quot;&gt;https://blog.aoya6i.com/mikrotik-crs310-1g-5s-4sin-upgrade-723-to-731&lt;/a&gt;&lt;/div&gt;
 

[MikroTik upgrade 7.2.3 to 7.3.1](https://blog.aoya6i.com/mikrotik-crs310-1g-5s-4sin-upgrade-723-to-731): 2022-07-17 &lt;p&gt;&lt;a target=&quot;_blank&quot; href=&quot;https://mikrotik.com/product/crs310_1g_5s_4s_in&quot;&gt;MikroTik Routers and Wireless - Products: CRS310-1G-5S-4S+IN&lt;/a&gt;&lt;/p&gt;
&lt;p&gt;&lt;/p&gt;
&lt;ul&gt;
&lt;li&gt;Hardware: CRS310-1G-5S-4S+IN&lt;/li&gt;
&lt;li&gt;Old Version: 7.2.3&lt;/li&gt;
&lt;li&gt;New Version: 7.3.1&lt;/li&gt;
&lt;/ul&gt;
&lt;h1 id=&quot;heading-changelogs&quot;&gt;changelogs &lt;/h1&gt;
&lt;p&gt;&lt;a target=&quot;_blank&quot; href=&quot;https://mikrotik.com/download/changelogs&quot;&gt;MikroTik Routers and Wireless - Software&lt;/a&gt;&lt;/p&gt;
&lt;p&gt;&lt;/p&gt;
&lt;pre&gt;&lt;code&gt;What&#39;s new in 7.3 &lpar;2022-Jun-06 11:38&rpar;:

&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; bonding - added &quot;lacp-user-key&quot; setting;
*&lt;/span&gt;&rpar; bonding - fixed LACP flapping for RB5009 and CCR2004-16G-2S+ devices;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; bridge - added more details for loop detection warning;
*&lt;/span&gt;&rpar; bridge - do not set VLAN on inactive port with a &quot;set&quot; command;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; bridge - fixed TCP, UDP port parsing for loop detect warning;
*&lt;/span&gt;&rpar; bridge - fixed packet marking for IP/IPv6 firewall;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; bridge - ignore VLAN tagged BPDU;
*&lt;/span&gt;&rpar; console - fixed &quot;terminal inkey&quot; command;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; l3hw - greatly improved route offloading speed;
*&lt;/span&gt;&rpar; l3hw - improved offloading for directly connected hosts on CRS305, CRS326-24G-2S+, CRS328, CRS318, CRS310;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; l3hw - improved offloading in cases of HW table overflow for CRS305, CRS326-24G-2S+, CRS328, CRS318, CRS310;
*&lt;/span&gt;&rpar; l3hw - log HW routes count and the shortest offloaded subnet prefix if the HW memory gets full;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; l3hw - offload only main routing table;
*&lt;/span&gt;&rpar; l3hw - optimized offloading when dealing with large volume of directly connected hosts;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; mlag - fixed MAC address moving between bridge ports;
*&lt;/span&gt;&rpar; ssh - added AES-GCM cipher support;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; ssh - fail non-interactive client after first invalid password;
*&lt;/span&gt;&rpar; ssh - fixed corrupt host key automatic regeneration;
&lt;span class=&quot;hljs-emphasis&quot;&gt;*&rpar; ssh - fixed private key usage after downgrade;
*&lt;/span&gt;&rpar; ssh - removed DSA public key authentication support;
&lt;/code&gt;&lt;/pre&gt;&lt;h2 id=&quot;heading-mlag&quot;&gt;MLAG &lt;/h2&gt;
&lt;p&gt;active-role: &lt;code&gt;secondary&lt;/code&gt; &lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/interface bridge mlag monitor once 
       status: connected
    system-id: 01:00:5e:90:10:00
  active-role: secondary
&lt;/code&gt;&lt;/pre&gt;
&lt;h2 id=&quot;heading-6kit5a6a44gu44kv44op44km44oj44oq44od44kv44ki44od44ox&quot;&gt;&lt;/h2&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/system/backup/cloud/remove-file number=0
/system/backup/cloud/upload-file action=create-and-upload password=


/system/backup/cloud/&lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt;
 0 name=&lt;span class=&quot;hljs-string&quot;&gt;&quot;cloud-20220717-191136&quot;&lt;/span&gt; size=31.4KiB ros-version=&lt;span class=&quot;hljs-string&quot;&gt;&quot;7.2.3&quot;&lt;/span&gt; date=jul/17/2022 19:11:38 status=&lt;span class=&quot;hljs-string&quot;&gt;&quot;ok&quot;&lt;/span&gt;
&lt;/code&gt;&lt;/pre&gt;
&lt;p&gt; status &lt;/p&gt;
&lt;h2 id=&quot;heading-44or44od44kx44o844k444gu5pu05paw56k66kqn&quot;&gt;&lt;/h2&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/system/package/update/check-for-updates
            channel: stable
  installed-version: 7.2.3
     latest-version: 7.3.1
             status: New version is available
&lt;/code&gt;&lt;/pre&gt;
&lt;h2 id=&quot;heading-44oa44km44oz44ot44o844oj&quot;&gt;&lt;/h2&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/system/package/update/download
            channel: stable
  installed-version: 7.2.3
     latest-version: 7.3.1
             status: Downloaded, please reboot router to upgrade it
&lt;/code&gt;&lt;/pre&gt;
&lt;h2 id=&quot;heading-44ki44od44ox44kw44os44o844oj6zal5ael&quot;&gt;&lt;/h2&gt;
&lt;p&gt;4 link &lt;/p&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/system/reboot
&lt;/code&gt;&lt;/pre&gt;
&lt;h2 id=&quot;heading-6kit5a6a44gu44kv44op44km44oj44oq44od44kv44ki44od44ox&quot;&gt;&lt;/h2&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;/system/backup/cloud/remove-file number=0
/system/backup/cloud/upload-file action=create-and-upload password=


/system/backup/cloud/&lt;span class=&quot;hljs-built_in&quot;&gt;print&lt;/span&gt;
 0 name=&lt;span class=&quot;hljs-string&quot;&gt;&quot;cloud-20220717-191136&quot;&lt;/span&gt; size=31.4KiB ros-version=&lt;span class=&quot;hljs-string&quot;&gt;&quot;7.2.3&quot;&lt;/span&gt; date=jul/17/2022 19:11:38 status=&lt;span class=&quot;hljs-string&quot;&gt;&quot;ok&quot;&lt;/span&gt;
&lt;/code&gt;&lt;/pre&gt;
 

[Vultr で Disk image をアップロードする場合](https://blog.aoya6i.com/vultr-disk-image-to-qcow2-convert-and-upload): 2022-07-16 &lt;p&gt;Vultr  Disk image 
VUltr  Disk image  http 
RAW image  qcow2  http &lt;/p&gt;
&lt;p&gt;&lt;a target=&quot;_blank&quot; href=&quot;https://www.vultr.com/ja/docs/best-practices-when-migrating-to-vultr/&quot;&gt;Best Practices when Migrating to Vultr - Vultr.com &lpar;&rpar;&lt;/a&gt;&lt;/p&gt;
&lt;ul&gt;
&lt;li&gt;&lt;/li&gt;
&lt;li&gt;Cumulus  KVM &lt;ul&gt;
&lt;li&gt;SUM256: &lt;code&gt;064fd2f767b36df871e70885b40141be76a903e063a0ba30fbf4dfa4f0a8ee4b&lt;/code&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;cat &amp;lt;&amp;lt;EOF&amp;gt; cumulus-linux-5.1.0-vx-amd64-qemu.sha256sum
064fd2f767b36df871e70885b40141be76a903e063a0ba30fbf4dfa4f0a8ee4b  cumulus-linux-5.1.0-vx-amd64-qemu.qcow2
EOF

wget https://d2cd9e7ca6hntp.cloudfront.net/public/CumulusLinux-5.1.0/cumulus-linux-5.1.0-vx-amd64-qemu.qcow2

sha256sum -c cumulus-linux-5.1.0-vx-amd64-qemu.sha256sum
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;&lt;code&gt;qemu-img&lt;/code&gt; &lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;apt install -y qemu-utils
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;qemu-img convert -f qcow2 -O raw cumulus-linux-5.1.0-vx-amd64-qemu.qcow2 cumulus-linux-5.1.0-vx-amd64-qemu.img
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;nginx &lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;apt install -y nginx
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;ufw &lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;ufw allow 80/tcp

ufw status verbose
&lt;/code&gt;&lt;/pre&gt;
&lt;ul&gt;
&lt;li&gt;&lt;/li&gt;
&lt;/ul&gt;
&lt;pre&gt;&lt;code class=&quot;lang-bash&quot;&gt;mv -v cumulus-linux-5.1.0-vx-amd64-qemu.img /var/www/html/cumulus-linux-5.1.0-vx-amd64-qemu.img

&lt;span class=&quot;hljs-built_in&quot;&gt;echo&lt;/span&gt; &lt;span class=&quot;hljs-string&quot;&gt;&quot;http://&lt;span class=&quot;hljs-subst&quot;&gt;$descriptionlpar;curl -sfSL ifconfig.me&rpar;&lt;/span&gt;/cumulus-linux-5.1.0-vx-amd64-qemu.img&quot;&lt;/span&gt;
&lt;/code&gt;&lt;/pre&gt;
 
<!-- BLOG-POST-LIST:END -->
