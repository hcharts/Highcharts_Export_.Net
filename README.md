# Highcharts 导出服务.Net版

## 部署
### 一、部署环境
```sh
.Net Framework 2.0+
IIS 6.0+
```
### 二、新建网站
#### 1.把导出服务的文件上传到服务器指定的目录
#### 2.以此目录作为网站的根目录，在IIS中新建网站
#### 3.假设网站的IP地址为192.168.1.100，端口为8080
### 三、如何调用服务
```sh
 $('#Chart').highcharts({
    // ... 省略代码
    exporting: {
        //url:"服务器地址:端口/Export.aspx"
        //url:"Server_Mechine_IP_Address:Port/Export.aspx"
        url:"192.168.1.100:8080/Export.aspx"
    }
 }
```
