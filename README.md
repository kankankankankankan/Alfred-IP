# Alfred-IP
自己用了所有的Workflow调用IP全部要么失效，要么不能达到自己索要功能，所以自己修改了一份，继David Ferguson作者上修改。

#2020.11.18更新代理配置，方便直接使用

#直接输入IP显示为两部分：
1.显示本地IP+地理位置
2.代理IP+地理位置

#如果出现代理IP没有显示
1.请安装插件后寻找PROXY=$(curl -x socks5://127.0.0.1:8001 --silent 'http://ipinfo.io' | /usr/local/bin/jq -r '.ip + "--" +.city + " " +.org')
2.修改`socks5://127.0.0.1:8001`为你本地的代理信息即可使用

`brew install jq`
