# 联行 #
 
************************

* 目录：
 - [1、联行地域列表查询接口](#t1)
 - [2、银行地域查询接口](#t2)
 - [3、银行列表查询接口](#t3)
 - [4、银行查询接口](#t4)
 - [5、联行列表查询接口](#t5)
 - [6、联行查询接口](#t6)

************************
### <span id="t1">1 </span>联行地域列表查询接口 ###

#### 1.1 接口描述 ####

查询联行地域列表信息。

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
xx| String | 非空 | 类目类型：<br/>1：省<br/>2：市/区/县
xx| String | 空 | 省ID


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
xx| String | 空 | 上级地域ID
xx| String | 空 | 上级地域名称
xx| String | 空 | 地域类型：<br/>1：省<br/>2：市/区/县


#### 1.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功

************************

### <span id="t2">2 </span>银行地域查询接口 ###

#### 2.1 接口描述 ####

查询银行地域信息。

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
xx| String | 空 | 上级地域ID
xx| String | 空 | 上级地域名称
xx| String | 空 | 地域类型：<br/>1：省<br/>2：市/区/县


#### 2.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功


************************

### <span id="t3">3 </span>银行列表查询接口 ###

#### 3.1 接口描述 ####

查询银行列表信息。

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
xx| String | 空 | CDE_FLG：<br/>0：<br/>1：

##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX< LIST >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 银行ID
xx| String | 非空 | 银行名称
xx| String | 非空 | 银行机构编码
xx| String | 非空 | CDE_FLG


#### 3.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功

************************

### <span id="t4">4 </span>银行查询接口 ###

#### 4.1 接口描述 ####

查询银行信息。

#### 4.2 接口概述 ####
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

#### 4.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 空 | 银行ID
xx| String | 空 | 银行机构编码


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 银行ID
xx| String | 非空 | 银行名称
xx| String | 非空 | 银行机构编码
xx| String | 非空 | CDE_FLG


#### 4.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功


************************

### <span id="t5">5 </span>联行列表查询接口 ###

#### 5.1 接口描述 ####

查询联行列表信息。

#### 5.2 接口概述 ####
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


#### 5.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 银行ID
xx| String | 空 | 省ID
xx| String | 空 | 市/区/县ID
xx| String | 空 | 联行名称关键字

##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX< LIST >：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 联行号
xx| String | 非空 | 联行名称
xx| String | 非空 | 所属银行ID
xx| String | 非空 | 所属银行名称
xx| String | 非空 | 所属银行机构编码
xx| String | 非空 | 所属省ID
xx| String | 非空 | 所属省名称
xx| String | 非空 | 所属市/区/县ID
xx| String | 非空 | 所属市/区/县名称
xx| String | 非空 | CDE_FLG


#### 5.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功


************************

### <span id="t6">6 </span>联行查询接口 ###

#### 6.1 接口描述 ####

查询联行信息。

#### 6.2 接口概述 ####
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

#### 6.3 参数说明 ####
##### 输入参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
uuid | String | 空 | 请求流水ID
sysId | String | 非空 | 系统编码
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 空 | 联行号


##### 响应参数： #####

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
code | String | 非空 | 返回码
message | String | 非空 | 返回信息
object | XXXX | 非空 | 业务参数

XXXX：

字段名称 | 类型 | 输入项 | 备注
---|---|---|---
xx| String | 非空 | 联行号
xx| String | 非空 | 联行名称
xx| String | 非空 | 所属银行ID
xx| String | 非空 | 所属银行名称
xx| String | 非空 | 所属银行机构编码
xx| String | 非空 | 所属省ID
xx| String | 非空 | 所属省名称
xx| String | 非空 | 所属市/区/县ID
xx| String | 非空 | 所属市/区/县名称
xx| String | 非空 | CDE_FLG


#### 6.4 响应码说明 ####

code | 描述
---|---
SES00000| 成功