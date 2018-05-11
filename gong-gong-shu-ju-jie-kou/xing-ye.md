# 行业 #
  
************************

* 目录：
 - [1、MCC类目列表查询接口](#t1)
 - [2、MCC列表查询接口](#t2)
 - [3、MCC查询接口](#t3)

************************
### <span id="t1">1 </span>MCC类目列表查询接口 ###

#### 1.1 接口描述 ####

查询MCC类目列表信息。

#### 1.2 接口概述 ####
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
xx| String | 非空 | 类目类型：<br/>1：一级类目<br/>2：二级类目
xx| String | 空 | 一级类目ID


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX< LIST >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 一级类目ID
xx| String | 非空 | 一级类目名称
xx| String | 空 | 二级类目ID
xx| String | 空 | 二级类目名称
xx| String | 空 | 类目类型：<br/>1：一级类目<br/>2：二级类目


#### 1.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功



************************

### <span id="t2">2 </span>MCC列表查询接口 ###

#### 2.1 接口描述 ####

查询MCC列表信息。

#### 2.2 接口概述 ####
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
xx| String | 非空 | 类目类型：<br/>1：一级类目<br/>2：二级类目
xx| String | 空 | 一级类目ID
xx| String | 空 | 二级类目ID


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX< LIST >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | MCCID
xx| String | 非空 | MCC名称
xx| String | 非空 | 一级类目ID
xx| String | 非空 | 一级类目名称
xx| String | 空 | 二级类目ID
xx| String | 空 | 二级类目名称


#### 2.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功



************************

### <span id="t3">3 </span>MCC查询接口 ###

#### 3.1 接口描述 ####

查询MCC信息。

#### 3.2 接口概述 ####
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

#### 3.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | MCCID


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | MCCID
xx| String | 非空 | MCC名称
xx| String | 非空 | 一级类目ID
xx| String | 非空 | 一级类目名称
xx| String | 非空 | 二级类目ID
xx| String | 非空 | 二级类目名称
xx| String | 非空 | BIZ_INFO
xx| String | 非空 | IND_INFO
xx| String | 非空 | BIZ_SCOPE



#### 3.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功