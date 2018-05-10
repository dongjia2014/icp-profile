# 地域  #
 
************************
************************
### 1 地域列表查询接口###

#### 1.1接口描述 ####

查询地域列表信息。

#### 1.2接口概述 ####
> 接口类：

<pre>

</pre>

> 接口方法名：

<pre>
    
</pre>

> 输入业务参数类型：

<pre>
com.suixingpay.common.rpc.v2.RpcRequest&lt;>
</pre>
> 输出业务参数类型：

<pre>
com.suixingpay.common.rpc.v2.RpcResponse&lt;>
</pre>


#### 1.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 地域类型：<br/>1：国家<br/>2：省<br/>3：市<br/>4：区/县
xx| String | 空 | 上级地域ID


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX< LIST >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 地域ID
xx| String | 非空 | 地域名称
xx| String | 非空 | CUP_CODE
xx| String | 非空 | 地域类型：<br/>1：国家<br/>2：省<br/>3：市<br/>4：区/县
xx| String | 空 | 上级类目ID
xx| String | 空 | 上级类目名称


#### 1.4响应码说明 ####

code | 描述
---|---
SES00000| 成功


************************

### 2 地域查询接口###

#### 2.1接口描述 ####

查询地域信息。

#### 2.2接口概述 ####
> 接口类：
<pre>

</pre>
> 接口方法名：
<pre>
    
</pre>
> 输入业务参数类型：
<pre>
com.suixingpay.common.rpc.v2.RpcRequest&lt;>
</pre>
> 输出业务参数类型：
<pre>
com.suixingpay.common.rpc.v2.RpcResponse&lt;>
</pre>

#### 2.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 地域ID


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 地域ID
xx| String | 非空 | 地域名称
xx| String | 非空 | CUP_CODE
xx| String | 非空 | 地域类型：<br/>1：国家<br/>2：省<br/>3：市<br/>4：区/县
xx| String | 空 | 上级类目ID
xx| String | 空 | 上级类目名称




#### 2.4响应码说明 ####

code | 描述
---|---
SES00000| 成功